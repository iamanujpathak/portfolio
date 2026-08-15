# Anuj Pathak — Portfolio

> Embedded & IoT engineer — I take connected products **from schematic to app store**: firmware, companion apps, and hardware, including **FCC-certified medical and safety-critical** devices. 10 years · Zephyr / Nordic / BLE · low-power · test-driven. Recently AI-accelerated.

## 📌 Quick links

| What | Where |
|---|---|
| Resume | [resume/resume.md](resume/resume.md) |
| CV (full record) | [cv/cv.md](cv/cv.md) |
| Case studies | [portfolio/](portfolio/) |
| Hire me | [Upwork ↗](https://www.upwork.com/freelancers/~01a418fb5c16816290) · [LinkedIn ↗](https://www.linkedin.com/in/anuj-pathak-b63076119/) |
| Consultancy | [BIII TECH ↗](https://biii.in) · [case studies ↗](https://biii.in/case-studies) |

## 🧰 Skills

- **MCUs:** ARM Cortex M0–M33 · Nordic nRF51/52/53/54/91 · STM32 F0–L4 · ESP32 family · PSoC 4/5/6 · SAMD21 · EFR32BG22 · DA14531 · low-cost Chinese MCUs
- **Connectivity:** BLE, WiFi, LoRa, Sub-GHz, Thread/OpenThread, Matter, Wirepas mesh
- **RTOS:** Zephyr (since 2020 — **upstream contributor**, [8 PRs merged into mainline](https://github.com/zephyrproject-rtos/zephyr/pulls?q=author%3Acx-anuj-pathak)) · FreeRTOS (since 2016) · ThreadX
- **Firmware:** bootloaders, OTA, low-power design, DAQ, drivers, kernel work
- **Protocols & buses:** SPI, I2C, UART, USB, RS485, CAN, I2S, MQTT, ZeroMQ, WebRTC
- **Languages & tools:** Embedded C, Python, Flutter, NodeJS, Java · CMake, OpenOCD, GDB, STM32Cube, Git
- **Practice:** TDD — automated SIL/HIL + interactive HIL & integration testing (ztest, Twister, Unity, CMock, FFF) · GitHub Actions CI/CD · AI-assisted development (Claude, Copilot, Gemini — daily over the last ~1.5 years)
- **Hardware design:** KiCad (PCB) · FreeCAD (enclosures)

## 💼 Flagship work

| Project | What I did | Outcome |
|---|---|---|
| [Clinical health wearable](portfolio/medical-wearable/README.md) | Dual-core nRF5340 multi-sensor firmware + C#/MAUI companion app | FCC-certified medical product: 30-day battery, 4× BLE throughput, full CI/CD |
| [CargoBeacon asset tracking](portfolio/cargobeacon-asset-tracking/README.md) | Wirepas mesh firmware (nRF52840) + EFR32 tracker + cross-platform apps | 5+ years battery life; multi-year Wirepas specialization |
| [A21 firmware library](portfolio/a21-firmware-library/README.md) | Code-protected binary library with a syscall-style ABI (SVC + vector table) | One board ships as multiple products — in commercial production |
| [Gyani — robotics learning platform](portfolio/robotics-learning-platform/README.md) | Bytecode-interpreting embedded OS + flowchart IDE + PCBs, solo | Watch it run: [product demo ↗](https://www.youtube.com/watch?v=RQ05I6xJ4js), [RC car ↗](https://www.youtube.com/watch?v=h7ZZa9d3q-w) |
| [GoGoPowerJuice rental system](portfolio/gogopowerjuice/README.md) | USB-C PD multi-charger hardware + full software stack (kiosk → rental app) | [Live product ↗](https://gogopowerjuice.com/) — deployed at 12+ partner venues, apps on both stores |
| [GPS hazard-warning system (Sunvis)](portfolio/gps-hazard-warning/README.md) | Dual-MCU safety device: GPS hazard detection + voice warnings + app w/ OTA | Complete safety product — hardware, firmware, app — solo |

## 🗂 More projects

| Project | Highlights |
|---|---|
| [OpenThread marine control](portfolio/thread-marine-control/README.md) | Replaced a collision-prone mesh; Thread+BLE on one nRF52840; ThingsBoard + Alexa; demoed in 4 months |
| [Lift monitoring system](portfolio/lift-monitoring/README.md) | CircuitPython→Zephyr productionization; replay-real-data algorithm harness cut testing by months |
| [Environmental monitoring node](portfolio/environmental-sensor/README.md) | LoRaWAN + BLE node — 3+ years on 2× AA lithium, MCUboot OTA |
| [Locomotive controller migration](portfolio/locomotive-can-controller/README.md) | Legacy CAN controller, feature-identical on nRF5340 incl. man-down auto-stop; BLE diagnostics |
| [Protein filtration control (TFF)](portfolio/protein-filtration-tff/README.md) | 50+ params real-time; PID rewrite: 3× faster steady state — line later used in COVID testing |
| [Blood slide heater](portfolio/blood-slide-heater/README.md) | Hand-tuned PID thermal profiling; delivered in 3 months, in production at labs |
| [Access control system](portfolio/access-control-system/README.md) | Multi-credential (RFID/Wiegand/HID/OSDP) controller — man-trap, tamper, RS485; 2× faster reaction, 5× faster OTA — in production |
| [Connected access control board](portfolio/connected-access-control-board/README.md) | STM32F4 + ESP32 dual-processor; OTA over both MQTT and BLE |
| [Connected vending kiosk](portfolio/vending-kiosk/README.md) | Flutter kiosk on Raspberry Pi + C/Python hardware control + cloud inventory sync |
| [BLE mesh home automation](portfolio/ble-mesh-home-automation/README.md) | Custom BLE beacon mesh + retrofit switchboard hardware; 2+ years running a real home |
| [MOSIP identity platform (PoC)](portfolio/mosip-identity-platform/README.md) | Biometric capture (fingerprint/iris/face) on RPi4 + PKI certificate-chain trust + Spring Boot backend |
| Long-range DAQ system (freelance) | BLE 5 Coded PHY sensor nodes at 16 µA (~1.5 yr on CR2032) + ESP32-C3 gateway |

Full project list in [cv/cv.md](cv/cv.md).

## ⭐ Client feedback

Verifiable reviews & ratings on my platform profiles:
- **Upwork:** [**$20K+ earned · 920 hours · 7 jobs** ↗](https://www.upwork.com/freelancers/~01a418fb5c16816290) · client-endorsed: *Committed to Quality, Detail Oriented, Collaborative*
- **Freelancer:** [**4.9 / 5** across 20 reviews ↗](https://www.freelancer.in/u/iamanujpathak) · member since 2019

> *"Amazing work with dedication to detail to make the project a success. I've worked multiple projects and very happy with the work and outcome. Would highly recommend and will continue to work on future projects and endeavors."*
> — 5.0★ on Upwork · [GoGoPowerJuice](portfolio/gogopowerjuice/README.md) Stage 1 (10-slot charging dock) — **Stage 3 is in progress today**

> *"It was an amazing experience working with BIII TECH LLP. Goes above and beyond to get the project completed. Communication was concise and prompt, and there was a sense of accountability to help achieve the goals of the project. This was the first time working with BIII TECH LLP, and it won't be my last. Highly recommend!"*
> — 5.0★ on Freelancer · the first [GoGoPowerJuice](portfolio/gogopowerjuice/README.md) USB-C PD board

> *"Great freelancer with expert skills, will hire him again in future."* — German client, 5.0★

## 📫 Contact

- Website: https://biii.in
- Email: iamanujpathak@gmail.com · anuj@biii.in
- Upwork: https://www.upwork.com/freelancers/~01a418fb5c16816290
- LinkedIn: https://www.linkedin.com/in/anuj-pathak-b63076119/
