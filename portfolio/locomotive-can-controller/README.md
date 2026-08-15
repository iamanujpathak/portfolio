# Locomotive Controller Migration (PoC) — Legacy CAN → nRF5340 + BLE

**Outcome in one line:** Migrated a legacy locomotive controller onto a new **nRF5340-based PCB** as a proof-of-concept — behaviorally **feature-identical** to the original CAN controller (including man-down operator safety), with an added **BLE backhaul and companion mobile app** to make testing and diagnostics far easier.

**Client:** A US rail / locomotive company *(name withheld — NDA)*
**Stack:** nRF5340 (nRF Connect SDK / Zephyr), CAN, BLE, Flutter
**Role:** Embedded developer — PoC firmware & migration (at Croxel Inc)
**Timeline:** 2022 – 2023

## The problem

The client ran a locomotive controller on older hardware and wanted to move it onto a modern Nordic-based platform — **without changing how it behaves.** In control systems for locomotives, "feature-identical" is a hard requirement: the migrated board has to speak the same CAN messages and drive the same logic as the unit it replaces, so it drops into the existing system transparently. At the same time, they wanted modern connectivity to make bring-up and diagnostics less painful than probing a CAN bus.

## What I built

- **A feature-identical re-implementation** of the legacy CAN controller on a new **nRF5340** PCB — matching the original's behavior, including CAN message encoding/decoding and multiplexing between the system's modules.
- **Man-down operator safety:** dual-accelerometer processing that detects when the operator has gone down and **automatically stops the locomotive** — a safety-critical feature carried faithfully from the legacy unit.
- **A BLE backhaul** added alongside the CAN interface — a wireless path into the controller that the legacy design never had.
- **A companion Flutter mobile app** that connects over BLE to exercise the controller, relay data, and diagnose behavior during testing — turning what used to be CAN-bus probing into something you can drive from a phone, including simultaneous BLE connections for multi-point diagnostics.

## The result

- A working **proof-of-concept** demonstrating the legacy controller's functionality on modern nRF5340 hardware, plus a wireless diagnostics path that didn't exist before.
- What this demonstrates: **legacy-system migration with behavioral fidelity, CAN bus firmware, and layering modern wireless (BLE) diagnostics onto an industrial control product.**

