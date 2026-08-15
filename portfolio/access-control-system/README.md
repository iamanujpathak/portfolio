# Access Control System — Multi-Credential Door & Perimeter Controller

**Outcome in one line:** Architected and built a feature-complete access-control platform on Atmel SAMD21 — man-trap, controlled access, maintenance mode, and tamper detection, with the full spread of industry credential technologies (RFID, 1-Wire, Wiegand, HID, OSDP) — **in production with a US security-hardware client**, with performance work that cut reaction time **2×** and OTA time **5×**.

**Stack:** Atmel SAMD21, Embedded C, RFID / 1-Wire / Wiegand / HID / OSDP, RS485, OTA, SPI graphical UI
**Role:** Research & Solution Architect — architecture, core libraries, foundational firmware (at IoTech Designs)
**Timeline:** 2019 – 2021 — my first project at IoTech

## The problem

Access control isn't one feature — it's a family of them, and they have to interlock reliably because the failure mode is a security breach. A single controller had to support multiple credential technologies (so it drops into existing installations), enforce access logic like **man-trap** interlocks and **maintenance mode**, detect **tampering**, support safe field updates, and network with other controllers over an industrial bus — all on a modest microcontroller.

## What I built

- **Access-control feature set:** man-trap (interlocked door pairs), controlled access, maintenance mode, tamper detection, and related access logic.
- **Multi-credential support:** RFID, 1-Wire, Wiegand, HID, and **OSDP** (the modern, supervised, encrypted access-control protocol) — so the controller speaks to virtually any reader in the field.
- **Rich I/O:** 16 resistive (supervised) inputs plus 4 wet and 4 dry contacts — enough to wire real doors, sensors, and relays without external expanders.
- **SPI-driven graphical user interface** for on-device status and interaction.
- **OTA firmware updates** and **RS485** networking for multi-controller installations.
- Built on **Atmel SAMD21**, with the firmware architecture and core libraries designed for reuse across the product line.
- **Hard real-time performance work:** a reactive event module dispatching events the moment they occur — **reaction time cut 2×** — plus an event-packing algorithm that lowers bus bandwidth and raises throughput.
- **Bootloader rework** cutting **OTA update time 5×**.

## The result

- A production-grade access-control platform covering the core commercial feature set on a single SAMD21 controller — **in production with a US security-hardware client**.
- What this demonstrates: **security-critical embedded systems, deep access-control domain knowledge (OSDP/Wiegand/HID), industrial I/O and networking, and architecture-for-reuse** — building the foundation a team then delivers on.
