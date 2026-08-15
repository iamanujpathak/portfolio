# Environmental Monitoring Node — LoRaWAN + BLE, 3+ Year Battery

**Outcome in one line:** A battery-powered environmental node (RH, temperature, lux, UV) that runs **3+ years on two AA lithium cells** — LoRaWAN telemetry plus a BLE companion app for configuration, missing-sample recovery, and MCUboot OTA.

**Client:** An environmental-monitoring company *(name withheld — NDA)*
**Stack:** nRF52840 (nRF Connect SDK / Zephyr), LoRaWAN, BLE, MCUboot, Flutter, 2× AA Li
**Role:** Embedded developer — firmware + companion app (at Croxel Inc)
**Timeline:** 2024 – 2025

## The problem

Some environments — archives, collections, controlled storage — have to be held within tight environmental bounds, and drift has to be caught early. That calls for sensor nodes that can be scattered through a space, report reliably over long range, and then be **left alone for years** — no wired power, no frequent battery swaps. Long battery life isn't a nice-to-have here; it's the whole product.

## What I built

### The sensor node
- **Multi-parameter environmental sensing:** relative humidity, temperature, lux, UV, and more — the readings needed to verify a space stays within its target conditions.
- **LoRaWAN backhaul:** periodic telemetry over long-range, low-power LoRaWAN, plus **downlink command/response** so a node can be queried and configured remotely, not just heard from.
- **Battery life as the headline spec:** low-power design across sensing, radio duty-cycling, and firmware to reach **3+ years on two AA lithium cells**.

### The companion app & serviceability
- **A Flutter companion app with BLE:** configure a node in the field, and **retrieve missing samples** over BLE — closing gaps in the LoRaWAN record so the dataset stays complete.
- **MCUboot OTA over BLE:** field firmware updates without pulling nodes off the wall.

## The result

- A deploy-and-forget environmental monitoring node: years of unattended operation, long-range reporting, and a phone-based path for setup, gap-filling, and updates.
- What this demonstrates: **ultra-long-life low-power design (3+ years on AA), LoRaWAN + BLE dual-connectivity firmware, robust data completeness (BLE sample recovery), and OTA serviceability** — plus the companion-app work to make it usable in the field.

