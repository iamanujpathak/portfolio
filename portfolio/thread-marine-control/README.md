# OpenThread Marine Control System — Hydraulic Anchors & Trolling Motors

**Outcome in one line:** Replaced a collision-prone legacy broadcast mesh with an **OpenThread** network for reliable control of marine hydraulic anchors and trolling motors, plus **ThingsBoard cloud and Alexa voice control** — designed, built, and demoed in **4 months**.

**Client:** A US marine-equipment manufacturer *(name withheld — NDA)*
**Stack:** nRF52840 (nRF Connect SDK / Zephyr), OpenThread, BLE, MPSL, Thread Border Router, CoAP, ThingsBoard cloud, Alexa Skill, Flutter
**Role:** Embedded developer — system design & firmware (first project at Croxel Inc)
**Timeline:** 2022, ~4 months

## The problem

The client's boats control hydraulic anchors and trolling motors wirelessly, but their **legacy broadcast-based mesh** suffered **on-air packet collisions** — messages stepping on each other over the air, causing dropped or delayed commands. For gear that physically moves a boat, an unreliable command path is a safety problem, not an annoyance. They needed a mesh that could carry addressed, acknowledged traffic without the collisions — and, increasingly, remote and voice control.

## What I built

- **An OpenThread-based control network** replacing the legacy broadcast mesh. Thread's IPv6 mesh with proper MAC-layer arbitration and addressed, retryable messaging **removed the on-air collisions** at the root — commands reach a specific actuator instead of being broadcast into contention.
- **Simultaneous BLE + Thread** on a single nRF52840 using Nordic's **MPSL** (Multiprotocol Service Layer) — so the device runs the Thread control mesh and BLE commissioning/local control at the same time on one radio.
- **Cloud integration via a Thread Border Router**, bridging the mesh to **ThingsBoard** over **CoAP** for remote monitoring and control.
- **An Alexa voice skill** for hands-free remote operation — "deploy the anchor" from the cloud path.
- **A Flutter app** to commission Thread network credentials onto the board over BLE — the onboarding step that gets a new device onto the mesh.

## The result

- Delivered in **~4 months**, culminating in a working demo: **hydraulic control driven from the ThingsBoard cloud.**
- What this demonstrates: **protocol migration to solve a real reliability problem, multiprotocol (Thread + BLE) firmware on a single SoC, Thread Border Router + cloud (CoAP/ThingsBoard) integration, and voice-assistant integration** — an end-to-end connected-product build.

