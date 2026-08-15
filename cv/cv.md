# Anuj Pathak — Curriculum Vitae

## Contact

- **Location:** Noida, Uttar Pradesh, India
- **Email:** iamanujpathak@gmail.com · anuj@biii.in
- **Website:** https://biii.in
- **LinkedIn:** https://www.linkedin.com/in/anuj-pathak-b63076119/
- **Upwork:** https://www.upwork.com/freelancers/~01a418fb5c16816290

## Professional summary

**Embedded & IoT engineer** taking connected products **from schematic to app store** — firmware, companion apps, and hardware. **10 years** across embedded/BLE/low-power systems (Zephyr since 2020 — **upstream contributor**), practicing **test-driven firmware development** (SIL/HIL, CI/CD). Delivered **FCC-certified medical, safety-critical, and industrial** products — from board bring-up and custom kernels to sensors running years on a coin cell. Recently AI-accelerated: integrated AI-assisted development into daily practice over the last ~1.5 years.

## Experience (full-time)

### Expert Embedded Engineer — Ciklum India (Chennai)
*Full-time employment · April 2026 – Present*

- Modernizing the firmware of a **shaver cleaning-center product line** for a global consumer-products brand — bringing a shipping appliance codebase up to current engineering practice — and building new features for an upcoming release.

### Lead Embedded Developer — Croxel Inc (USA)
*Full-time consultancy · remote · April 2022 – April 2026*

- Delivered Zephyr RTOS (nRF Connect SDK) firmware across nRF52 / nRF53 / nRF54 products — including the **FCC-certified clinical health wearable**, the **OpenThread marine control system**, the **locomotive controller migration**, the **lift-monitoring productionization**, and the **3+ year LoRaWAN environmental node** (all under [Projects](#projects) below).
- Earned **upstream Zephyr contributor** status — **8 PRs merged** into the mainline Zephyr RTOS project (drivers, Bluetooth services, UART).
- Built the companion apps alongside the firmware: Flutter, and a production **Xamarin → .NET MAUI** migration.

### Senior Embedded Developer — Techno Brains Group (IN)
*Full-time consultancy (via Eureka Solutions) · remote · November 2021 – April 2022*

- Built a **MOSIP-compliant identity-management PoC** (the open national-ID standard, à la UIDAI): biometric capture — fingerprint, iris, face — on a Raspberry Pi 4 device server with **certificate-chain trust**, plus a Spring Boot management backend ([case study](../portfolio/mosip-identity-platform/README.md)).

### AVP, Research & Solution Architect — IoTech Designs, Noida
*Full-time employment · September 2019 – November 2021*

- Owned research and architecture for the product line: the **SAMD21 multi-credential access-control platform** (in production; 2× faster reaction, 5× faster OTA), its **STM32F4 + ESP32 connected variant**, the **A21 code-protected binary-library architecture** (shipping in commercial products), and the **vending kiosk platform** — building foundations that delivery teams then shipped.
- Developed the core libraries behind those products; coordinated teams and timelines as AVP.

### L3 Firmware Developer — Lattice Innovations, Okhla
*Full-time employment · February 2019 – August 2019*

- Delivered a precision **blood slide heater** for a medical client in 3 months — hand-tuned PID with heater + fan actuation and multi-step thermal profiling; in production at local labs ([case study](../portfolio/blood-slide-heater/README.md)).
- Built the **TFF protein-filtration control library** for a US bioprocessing system — 50+ parameters in real time; PID rewrite: steady state **3× faster**, error **2× lower** ([case study](../portfolio/protein-filtration-tff/README.md)).
- Managed embedded projects and API alignment with the web team.

### Co-Founder — Bhawna Infinity Tech, Delhi
*Founder · full-time · August 2016 – January 2019*

- Built **Gyani**, a complete no-code robotics learning platform, solo: bytecode-interpreting embedded OS on nRF51822, flowchart-to-bytecode IDE (JavaFX + Android), OTA bootloader, and KiCad PCBs — completed beyond PoC ([case study](../portfolio/robotics-learning-platform/README.md) · [demo](https://www.youtube.com/watch?v=RQ05I6xJ4js)).

## Parallel & consulting engagements

*Part-time work carried out alongside the full-time roles above.*

### Embedded Consultant — CargoBeacon AB (EU) — [case study](../portfolio/cargobeacon-asset-tracking/README.md)
*Part-time consultancy · remote · April 2021 – Present (parallel to full-time roles)*

- Designed an **ultra-low-power beacon asset tracker** on Silicon Labs EFR32 — **5+ years battery life**.
- Developed **Wirepas Mesh** firmware on nRF52840 across the protocol's node roles (mesh routing, positioning, ultra-low-power sleep, secure provisioning) — specialist Wirepas experience.
- Built **cross-platform Flutter apps** (Android/iOS/Windows/macOS) — later split with a shared reusable **Rust** core — with device interaction over **BLE and NFC** (firmware + app); established **CI/CD** and automated + manual firmware test suites.

### Freelance — Upwork / Freelancer & direct clients
*Part-time consultancy · ongoing (parallel)*

- Selected freelance embedded/IoT engagements — see **Projects → Freelance projects** below.

## Education

- **M.Tech (DC)** — AIACT&R (GGSIPU), Aug 2014 – Jul 2016
- **B.Tech** — NIEC Delhi, Aug 2010 – Jul 2014

## Open source

- **Zephyr RTOS — upstream contributor.** **8 pull requests merged** into the mainline Zephyr project (9 submitted), spanning device drivers (I2S, DMA, LED, sensor), Bluetooth services (Current Time, Heart Rate), and a generic UART property refactor. Verifiable → [merged PRs ↗](https://github.com/zephyrproject-rtos/zephyr/pulls?q=author%3Acx-anuj-pathak)

## Publications & research

- **"Ant Colony Optimization and Excess Energy Calculations Based Fast Converging Energy Efficient Routing Algorithm for WSNs"** — Springer, August 2019, co-authored with Dr. Aarti Jain. Energy-efficient ACO routing for wireless sensor networks.

## Skills

### Microcontrollers (hands-on)
- **Nordic:** nRF51 / nRF52 / nRF53 / nRF54, nRF91
- **STM32:** F0/F1/F2/F4, L0/L4
- **Espressif:** ESP32 / C3 / C5 / C6 / S3
- **Cypress PSoC** 4/5/6, **SAMD21**, **EFR32BG22** (Silicon Labs), **DA14531** (Dialog/Renesas)
- **Low-cost Chinese MCUs:** Puya, GigaDevice, WCH (CH570/572), HK, MM, etc.

### SBCs & compute modules
- Raspberry Pi 3/4, Pine A64 LTS, Quectel SC200R

### RTOS
- **Zephyr RTOS** (since 2020) — **upstream contributor** ([8 PRs merged](https://github.com/zephyrproject-rtos/zephyr/pulls?q=author%3Acx-anuj-pathak)) · **FreeRTOS** (since 2016) · **ThreadX** (one project)

### Peripherals & connectivity
- **BLE** (Advertising Extensions, Coded PHY, FCC DTM), WiFi, LoRa, Sub-GHz, NFC, RFID
- **USB** (MSC, CDC, HID, Vendor), CAN, RS485, OSDP, UART/USART, SPI, I2C, I2S, ADC, DMA, RTT
- WS2812B

### IoT protocols
- MQTT, ZeroMQ, REST, WebRTC, OpenThread, Matter, Wirepas, CoAP, LoRaWAN

### Firmware specialties
- Bootloaders (incl. secure & two-stage), OTA updates, low-power design, DAQ, kernel development, BLE mesh, edge algorithms

### AI & engineering practice
- **AI-assisted development (last ~1.5 years):** integrated Claude, GitHub Copilot, and Gemini into daily practice on current client work (Ciklum, CargoBeacon, and late-stage features on prior products). Largest gains in unit-test generation, scaffolding, and boilerplate — always reviewed against the architecture discipline below.
- **Architecture-first:** modular, flexible system designs that fulfill current requirements while staying extensible for future needs — the discipline that makes AI-assisted output safe to integrate.
- **Test-driven development:** modular architecture verified through **SIL** (software-in-the-loop, automated), **HIL** (hardware-in-the-loop, automated), **IHIL** (interactive hardware-in-the-loop), and integration testing — full test coverage from day one.
- **Test frameworks:** Zephyr ztest, Twister, Unity, CMock, FFF.
- **CI/CD:** GitHub Actions pipelines — unit-test verification, test builds, release generation, and deployment to servers and the Play Store.
- **On-device intelligence:** edge analytics algorithms (lift-health monitoring metrics), dual-accelerometer man-down detection.

### IDEs & tools
- VSCode, Eclipse, Keil, PSoC Creator, Simplicity Studio 5, ESP-IDF, STM32Cube IDE/MX
- ARM-GDB, OpenOCD, PyOCD, Git, Make, CMake, Bash

### Hardware design
- **KiCad** — PCB design (fabricated & shipped boards) · **FreeCAD** — enclosure design

### Programming languages
- C (primary), C++, Python, Java, Flutter/Dart, NodeJS, Kotlin (beginner)

## Projects

### Lift monitoring system — lift/elevator analytics client (US, at Croxel) — [case study](../portfolio/lift-monitoring/README.md)
- Migrated the client's lift floor/trip-detection algorithm from a **CircuitPython** prototype to production **Zephyr** firmware on **STM32L0**, applying production lessons from prior projects.
- Built an **Algorithm Simulation Framework (ASF):** compiles the *real* C algorithm and drives it via **Python FFI** against datasets recorded from real trips — **iteratively tuning and optimizing** floor/trip detection offline until satisfactory, **cutting device-testing cycles by months**. (An optimization harness, not a pass/fail SIL test.)
- Sensors: accelerometer + barometer; SD-card logging; **NB-IoT cellular** backhaul (Blues Notecard); low-power optimized for battery operation. Shipped with an optimized algorithm.

### Environmental monitoring node — environmental-monitoring client (at Croxel) — [case study](../portfolio/environmental-sensor/README.md)
- Battery-powered multi-parameter environmental node (RH, temperature, lux, UV) on nRF52840 (nRF Connect SDK) for controlled/preservation environments.
- **LoRaWAN** telemetry with downlink command/response; **3+ years battery life on 2× AA lithium** through low-power design.
- Flutter companion app over **BLE**: field configuration and **missing-sample retrieval** (gap-filling the LoRaWAN record); **MCUboot OTA over BLE**.

### Clinical health wearable — firmware + companion app (US medical-wearable client, at Croxel) — [case study](../portfolio/medical-wearable/README.md)
*The longest and most complete engagement of my Croxel tenure (multi-year).*
- **Wristband firmware** on dual-core **nRF5340** (App + Net cores, IPC): multi-sensor capture (IMU, accelerometer, magnetometer, barometer, PPG for BP/SpO₂) to 1 Gb NAND, with timing synchronization and data-integrity checks critical to the downstream data-science analysis.
- Raised **BLE throughput ~300 kbps → ~1.2 Mbps (≈4×)**; vendor-specific USB protocol; ~**30-day battery life**.
- **MCUboot** dual-bank OTA; **coredump** in-field crash diagnostics; **Direct Test Mode** firmware for **FCC certification**.
- **Full test coverage + CI/CD** to prevent production bugs; carried through the full production lifecycle (evaluation → development → production kits).
- **Companion app (C#/.NET MAUI):** migrated the production app from Xamarin to MAUI, raised BLE throughput to match, implemented and tested background sync.

### OpenThread marine control system — US marine-equipment client (at Croxel) — [case study](../portfolio/thread-marine-control/README.md)
- Replaced a collision-prone legacy broadcast mesh with an **OpenThread** network to control hydraulic anchors and trolling motors — eliminating the on-air packet collisions of the legacy system.
- nRF52840 (nRF Connect SDK), **MPSL** for simultaneous BLE + Thread; Thread Border Router bridging to **ThingsBoard** cloud over CoAP; **Alexa voice skill** for remote control.
- Flutter app to commission Thread credentials over BLE. Delivered in **4 months**; demoed hydraulic control end-to-end from the ThingsBoard cloud.

### Locomotive controller migration (PoC) — US rail/locomotive client (at Croxel) — [case study](../portfolio/locomotive-can-controller/README.md)
- Migrated a legacy locomotive controller to a new **nRF5340** PCB (nRF Connect SDK) — behaviorally **feature-identical** to the original CAN controller: CAN message encoding/decoding and multiplexing between modules.
- **Man-down operator safety:** dual-accelerometer processing that auto-stops the locomotive if the operator goes down — carried faithfully from the legacy unit.
- Added a **BLE backhaul** and a Flutter companion app (simultaneous BLE connections, data relay) to ease testing and diagnostics.

### MOSIP identity-management platform (PoC, at Techno Brains) — [case study](../portfolio/mosip-identity-platform/README.md)
- MOSIP-compliant device server on Raspberry Pi 4 (Java + C) capturing **fingerprint, iris, and face** biometrics — the open standard behind national-ID programs (comparable to UIDAI/Aadhaar).
- **Certificate-chain and authority verification** securing identity data through store / load / verify at every pipeline stage.
- Management server in **Java Spring Boot**; background desktop service for device monitoring; desktop UI client.

### Access control system — multi-credential door/perimeter controller (first project at IoTech) — [case study](../portfolio/access-control-system/README.md)
- Feature-complete access-control platform on **Atmel SAMD21**: man-trap, controlled access, maintenance mode, tamper detection.
- Multi-credential support — **RFID, 1-Wire, Wiegand, HID, OSDP**; 16 resistive inputs + 4 wet / 4 dry contacts; SPI graphical UI.
- OTA firmware updates and RS485 networking for multi-controller installations.
- Performance work: hard real-time reactive event dispatch (**2× faster reaction**), event-packing for bandwidth/throughput, bootloader rework (**5× faster OTA**). **In production with a US security-hardware client.**

### Connected access control board — STM32F4 + ESP32 (at IoTech) — [case study](../portfolio/connected-access-control-board/README.md)
- Single-door connected variant on a **dual-processor architecture**: STM32F4 host for access-control logic, ESP32 for WiFi/BLE connectivity.
- MQTT cloud control; **OTA over both MQTT and BLE**. Same access-control feature set, cloud-native single-board deployment.

### A21 — code-protected binary firmware library (first architecture role, at IoTech) — [case study](../portfolio/a21-firmware-library/README.md)
- Reusable access-control core sealed as a **precompiled binary library** at a fixed location — not source, not a linkable static lib — for genuine code protection.
- **Syscall-style ABI:** services exposed via a vector table, entered through a software interrupt (SVC), with parameters and return codes marshalled by stack-frame manipulation — a stable binary interface with no app↔library linking (OS syscall model on bare metal).
- Library owns and arbitrates all resources (GPIO/I2C/SPI/ADC + logical modules like card readers/inputs/outputs); apps are Arduino-simple C holding only business logic.
- **One board → multiple products:** same library, different business-logic apps. Two-stage bootloader (bootloader → library → app); HAL wrapper for future MCU swaps; event-based, layered, with channel support.
- In commercial production — used in shipping access-control products in the field.

### Connected vending kiosk — intelligent-vending client (at IoTech) — [case study](../portfolio/vending-kiosk/README.md)
- Flutter kiosk UI on Raspberry Pi in locked single-app mode (bash install/autoboot); C + Python peripheral-control layer over WebSocket IPC.
- Drives machine subsystems (dispense motors, refrigeration, heater, drop/weight sensors); BLE peripheral on Pi & Pine A64 via GDBus.
- **Cloud-connected:** fetch inventory → build cart → dispense → write inventory back to cloud, keeping every machine in sync.

### Protein filtration control library — bioprocessing TFF system (medical, at Lattice Innovations) — [case study](../portfolio/protein-filtration-tff/README.md)
- Multi-threaded Java (Windows) control library for a US bioprocessing manufacturer's tangential-flow-filtration (TFF) system — real-time monitoring and control of 50+ parameters, with APIs driving the product's GUI front end.
- Profiled filtration/diafiltration processing with continuous input/output flow and pressure monitoring.
- Proposed and implemented an advanced PID control algorithm: steady state **3× faster**, steady-state error **2× lower**. Same instrument line later used in COVID-19 testing.

### Blood slide heater (medical, at Lattice Innovations) — [case study](../portfolio/blood-slide-heater/README.md)
- Precision blood-slide preparation instrument: PID loop driving a 12 V heat bead (high-frequency switching electronics) and a cool-down fan — coefficients hand-tuned through iterative data collection to minimize overshoot, undershoot, and steady-state error.
- **Thermal profiling engine**: operator-defined (temperature, duration) step arrays executed unattended; state machine + HMI GUI; every run's temperature trace logged to a file on USB for compliance records.
- Delivered within **3 months**; in production use at local labs.

### Gyani — robotics learning platform (startup) — [case study](../portfolio/robotics-learning-platform/README.md)
- Product: **Gyan-Yantra** (device) + **Gyan-Matra** (app). Demo videos: [walkthrough](https://www.youtube.com/watch?v=RQ05I6xJ4js), [LED blink](https://www.youtube.com/watch?v=FUhqrbocwGk), [RC car](https://www.youtube.com/watch?v=h7ZZa9d3q-w).
- Java-like bytecode interpreter in Embedded C on **FreeRTOS** (nRF51822, nRF5 SDK 12) — an embedded OS executing student programs on the fly from RAM; custom bytecode instruction set covering peripheral init and control.
- Flowchart IDE with conditional paths: **JavaFX desktop + Kotlin/Java Android apps on a shared Java core**, compiling flowcharts to bytecode, delivered over a custom BLE / USB-UART protocol.
- **Dual-bank bootloader** with OTA over BLE/USB-UART and firmware anti-cloning protection; board and module PCBs in KiCad — fabricated, assembled, tested.
- Completed and moved beyond PoC; venture wound down on marketing, not engineering.

### BLE beacon mesh home automation (independent project) — [case study](../portfolio/ble-mesh-home-automation/README.md)
- Retrofit smart-switch system for traditional modular switchboards: 5×5 cm main board (controller, custom AC-DC, EEPROM, solid-state switching) driving up to **16** 2.5×5 cm switch modules — collapsing whole-house BOM.
- Custom **BLE beacon mesh** protocol on nRF51822 (nRF5 SDK 12) — hubless, cloudless whole-house control; Android app joins the mesh directly for live status and switching.
- PoC deployed in own home: **2+ years of continuous daily operation** (single failure: AC-DC stage fused by an external inverter short). Halted before mass production by funding.

### GPS hazard-warning system — mountain-terrain driver assistance (freelance) — [case study](../portfolio/gps-hazard-warning/README.md)
- Complete GPS-based hazard-warning device for mountain roads: tracks vehicle position, detects upcoming terrain hazards, and plays **pre-recorded voice warnings** for the driver.
- **Dual-MCU (STM32 + ESP32)** hardware + firmware; **dual audio amplifiers (20 W + 5 W)** and microphone; display, NAND + SD storage, RS485.
- **Companion Flutter app** to download audio content from the server to the device and perform **OTA** updates. For **Sunvis** (India), late 2022 – 2023.

### GoGoPowerJuice — power-bank rental system (freelance) — [case study](../portfolio/gogopowerjuice/README.md)
*Public freelance engagement (visible on Upwork / Freelancer).*
- **Charger hardware:** multi-channel USB-C Power Delivery chargers (5- and 10-channel) on **Cypress (Infineon) PD ICs**, all fed from a single **180 W** adapter — intelligent power budgeting across channels; PCB design.
- **Full software system:** Flutter vending kiosk app, backend, frontend, and the customer rental mobile app — the complete rent-a-charger platform apart from the vending enclosure.

### Freelance projects (selected)
*Client names withheld (NDA); recorded privately. Descriptive labels used below.*
- **Modular sensor platform (2022):** a sensor board (started on **PSoC** in 2022, later migrated to **ESP32-C5**) with pluggable USB-C sensor modules — IMU, accelerometer, temp/RH, infrared camera, laser distance, ADC — plus a Flutter app streaming data live from the device. For a California sensor startup.
- **Secure encrypted bootloader on ThreadX:** designed a secure, encrypted bootloader for a sports/athletics-tech client's board.
- **NFC firmware bootloader + low-power fix:** NFC-based bootloader (STM32F446RE + ST25DV) with an Android/iOS app to install binaries over NFC, plus a low-power bug fix. For a European NFC smart-lock (drawer-lock) maker.
- **Long-range data-collection system (freelance):** BLE 5 (**Coded PHY**) nRF52 sensor nodes drawing as low as **16 µA** (~1.5 years on CR2032) with an **ESP32-C3** gateway relaying to the server; PCBs in KiCad.
- **Pressure-based weight device (2021):** low-power, high-precision weight/load measurement for kitchen appliances on nRF52832 (deep-sleep), with a BLE interface and OLED display. For a kitchen-appliance client.
- **PID fluid dispenser (2020):** digital PID control for a PCB-industry electronic fluid dispenser (precise metered dispensing). For a dispensing-equipment client.
- **Lightsaber toy (2020):** firmware for a Star Wars-style lightsaber toy (motion / LED / sound). For a German consumer-electronics client.
- Ultra-low-power BLE beacon: connected-state consumption as low as **8 µA**.
- Firmware flash utility in JavaFX and Flutter; Wirepas Mesh and Zephyr RTOS application development.

## Languages

- Hindi, English

## Hobbies

- Chess, learning
