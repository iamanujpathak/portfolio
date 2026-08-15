# Anuj Pathak

**Embedded & IoT Engineer — Firmware · Apps · Hardware | Zephyr · Nordic · BLE · Low-Power · Medical/Safety-Critical**
Noida, India · iamanujpathak@gmail.com · [biii.in](https://biii.in) · [LinkedIn](https://www.linkedin.com/in/anuj-pathak-b63076119/) · [Upwork](https://www.upwork.com/freelancers/~01a418fb5c16816290)

## Summary

Embedded & IoT engineer who takes connected products **from schematic to app store** — firmware, companion apps, and hardware. **10 years** across embedded/BLE/low-power systems (Zephyr since 2020 — **upstream contributor**), practicing **test-driven firmware development**. Shipped **FCC-certified medical, safety-critical, and industrial** products — from board bring-up and custom kernels to sensors running **1.5+ years on a coin cell**. Recently AI-accelerated.

## Skills

**RTOS:** Zephyr / nRF Connect SDK (since 2020; **upstream contributor — 8 merged PRs**), FreeRTOS (since 2016), ThreadX ·
**MCUs:** Nordic nRF51/52/53/54/91, STM32 F0–L4, ESP32, PSoC 4/5/6, EFR32BG22, DA14531, SAMD21 ·
**Connectivity:** BLE (AE, Coded PHY, FCC DTM), Thread/Matter, Wirepas mesh, LoRaWAN, NFC, WiFi, CAN, USB, RS485/OSDP ·
**Specialties:** bootloaders (secure, two-stage), OTA, low-power design, DAQ, edge algorithms ·
**Languages & tools:** C, C++, Python, Java, Flutter · CMake, OpenOCD/PyOCD, GDB, KiCad, FreeCAD, Git ·
**Practice:** TDD — automated SIL/HIL, interactive HIL & integration testing · ztest, Twister, Unity, CMock, FFF · GitHub Actions CI/CD (tests → builds → releases → deploy) · AI-assisted development (Claude, Copilot, Gemini — daily over the last ~1.5 years)

## Experience (full-time)

### Expert Embedded Engineer — Ciklum India (Chennai)
*Full-time employment · April 2026 – Present*
- Modernizing shaver cleaning-center firmware for a global consumer-products brand, and building new features for an upcoming release.

### Lead Embedded Developer — Croxel Inc (USA)
*Full-time consultancy · remote · April 2022 – April 2026*
- Delivered multi-year firmware for a **clinical health wearable** on dual-core nRF5340 — multi-sensor capture (IMU/PPG/baro), timing sync & data integrity, FCC certification (DTM), MCUboot OTA, ~30-day battery, and a ~4× BLE throughput gain (300 kbps → 1.2 Mbps) — with full test coverage and CI/CD; also migrated its companion app from Xamarin to .NET MAUI with background sync.
- Replaced a marine client's collision-prone broadcast mesh with an OpenThread + BLE system (MPSL, one nRF52840), with ThingsBoard cloud and Alexa voice control — demoed in 4 months.
- Migrated a legacy CAN locomotive controller onto nRF5340 — feature-identical, including man-down auto-stop safety — adding a BLE backhaul and a Flutter diagnostics app.
- Productionized a lift-monitoring algorithm (CircuitPython → Zephyr on STM32L0, NB-IoT, battery-optimized) and built an Algorithm Simulation Framework — compiling the real C algorithm and replaying recorded elevator trips via Python FFI to iteratively optimize floor/trip detection offline — cutting device-testing cycles by months.
- Built a LoRaWAN + BLE environmental monitoring node (nRF52840) engineered for 3+ years on 2× AA lithium, with MCUboot OTA over BLE and a Flutter app for field config and gap-filling missing samples.
- **Upstream Zephyr RTOS contributor** — [8 PRs merged](https://github.com/zephyrproject-rtos/zephyr/pulls?q=author%3Acx-anuj-pathak) into the mainline project (drivers, Bluetooth services, UART).

### Senior Embedded Developer — Techno Brains Group (IN)
*Full-time consultancy (via Eureka Solutions) · remote · November 2021 – April 2022*
- Built a MOSIP-compliant identity-management PoC (the open national-ID standard, à la UIDAI): biometric capture (fingerprint/iris/face) on a Raspberry Pi 4 device server (Java/C) with certificate-chain trust, plus a Spring Boot management server.

### AVP, Research & Solution Architect — IoTech Designs, Noida
*Full-time employment · September 2019 – November 2021*
- Owned research and architecture; built core libraries and foundational firmware, then handed over to delivery teams.
- Architected a multi-credential access-control platform on SAMD21 (RFID/1-Wire/Wiegand/HID/OSDP, man-trap, tamper detection, OTA, RS485), plus a connected STM32F4+ESP32 dual-processor variant (WiFi/BLE, MQTT, OTA over both MQTT and BLE).
- Designed **A21** (first architecture role): a code-protected binary firmware library with a syscall-style ABI (SVC + vector table, stack-frame parameter passing) letting one access-control board ship as multiple products — each app is simple business-logic C on the shared library; HAL layer for MCU portability.
- Delivered a connected vending kiosk: Flutter UI on Raspberry Pi (locked kiosk mode) with a C/Python peripheral-control layer and cloud inventory sync — full-stack embedded-Linux appliance.
- On that SAMD21 platform, cut reaction time 2× (hard real-time event dispatch) and OTA time 5× (bootloader rework) — in production with a US security-hardware client.

### L3 Firmware Developer — Lattice Innovations, Okhla
*Full-time employment · February 2019 – August 2019*
- Delivered a precision blood slide heater for a medical client in 3 months: hand-tuned PID (heater + fan), multi-step thermal profiling, HMI GUI, per-run USB compliance logs — in use at local labs.
- Built the multi-threaded Java control library for a bioprocessing protein-filtration (TFF) system — real-time control of 50+ parameters; PID rewrite reached steady state 3× faster at 2× lower error. (Same instrument line later used in COVID-19 testing.)
- Managed embedded projects and API alignment with the web team.

### Co-Founder — Bhawna Infinity Tech, Delhi
*Founder · full-time · August 2016 – January 2019*
- Built a no-code robotics learning platform for kids solo: bytecode-interpreting embedded OS on nRF51822/FreeRTOS executing from RAM, flowchart-to-bytecode compiler (JavaFX + Android, shared Java core), dual-bank OTA bootloader with anti-cloning, KiCad PCBs.

## Parallel / consulting (alongside full-time roles)

### Embedded Consultant — CargoBeacon AB (EU)
*Part-time consultancy · remote · April 2021 – Present*
- Designed a 5+ year ultra-low-power EFR32 beacon tracker and developed **Wirepas mesh** firmware on nRF52840 across the protocol's node roles (routing, positioning, low-power sleep, provisioning).
- Built cross-platform **Flutter** apps (Android/iOS/Windows/macOS), later split with a shared **Rust** core, with CI/CD and automated + manual firmware test suites.

### Freelance — embedded/IoT contracts (Upwork, Freelancer & direct)
*Part-time consultancy · ongoing*
- **GoGoPowerJuice** (public engagement): designed multi-channel USB-C PD power-bank chargers (Cypress ICs, 5/10-channel, single 180 W supply) **and** the full software system — Flutter vending kiosk, backend, frontend, and customer rental app.
- **Sunvis** (2022–23): complete GPS hazard-warning system for mountain roads — dual-MCU (STM32 + ESP32) safety device with GPS hazard detection, pre-recorded voice warnings, dual audio amplifiers (20 W + 5 W), and a companion Flutter app for audio provisioning and OTA.
- Other engagements: long-range BLE 5 sensors (16 µA, Coded PHY, ESP32-C3 gateway), NFC bootloader (STM32 + ST25DV) with iOS/Android app, ultra-low-power BLE beacon (8 µA connected), Wirepas BLE mesh, firmware flash utilities.

## Education & research

- **M.Tech (DC)** — AIACT&R (GGSIPU), 2014–2016 · **B.Tech** — NIEC Delhi, 2010–2014
- Springer publication (2019): energy-efficient ACO routing algorithm for WSNs.
