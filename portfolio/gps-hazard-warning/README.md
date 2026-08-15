# GPS Hazard-Warning System — Mountain-Terrain Driver Assistance

**Outcome in one line:** Developed a complete GPS-based **hazard-warning system for mountain roads** — a dual-MCU (STM32 + ESP32) device with a dual audio-amplifier subsystem that tracks the vehicle's position, detects upcoming terrain hazards, and plays **pre-recorded voice warnings** to assist the driver.

**Client:** **Sunvis** (India) — vehicle-safety / driver-assistance *(named with permission — no NDA)*
**Stack:** STM32 + ESP32 (dual-MCU), GPS, dual audio amplifiers (20 W + 5 W), microphone, RS485, display, NAND + SD card
**Role:** Freelance embedded developer — complete hardware + firmware
**Timeline:** Late 2022 – late 2023 (~1 year, direct engagement)

## The problem

Mountain roads are full of **location-specific hazards** — blind curves, steep drops, landslide-prone stretches — that a driver unfamiliar with the terrain can't anticipate. The idea: a device that always knows **where the vehicle is**, knows **what's coming up on the road ahead**, and **speaks a warning in time** for the driver to react. A co-pilot that never stops watching the road.

## What I built

A complete embedded product — hardware and firmware:

- **Dual-MCU architecture (STM32 + ESP32):** an STM32 handling the real-time control and peripherals, with an ESP32 for connectivity — partitioning deterministic control from the wireless/compute workload.
- **GPS positioning + hazard detection:** continuously track the vehicle's location and match it against known hazard points along the route, so a warning fires *before* the hazard, not at it.
- **Dual audio-amplifier subsystem — 20 W + 5 W:** drives the voice warnings at the right level for the cabin (and/or an external speaker), with a **microphone** for the driver.
- **Pre-recorded warning playback:** context-appropriate voice warnings stored on device and played based on position and upcoming hazard.
- **Rich peripheral set:** a **display** for status/UI, **NAND + SD-card** storage (audio clips, hazard data, logs), and **RS485** for wired integration.
- **Companion Flutter app:** downloads audio content from the server onto the device — so warning clips can be provisioned and updated in the field — and handles **OTA firmware updates**.

## The result

- A complete, working driver-assistance safety device — from schematic through firmware — for a genuinely useful purpose: keeping drivers safer on dangerous mountain terrain.
- What this demonstrates: **complete embedded-product engineering** — dual-MCU architecture, a full audio subsystem, GPS hazard logic, and a companion app with OTA — a safety-critical product delivered solo: hardware, firmware, and app.

