# Clinical Health Wearable — Wristband Firmware + Companion App

**Outcome in one line:** Full-lifecycle firmware for an **FCC-certified clinical health wristband** on the dual-core nRF5340 — **30-day battery, 4× BLE throughput, MCUboot OTA, full test coverage + CI/CD** — plus its C#/.NET MAUI companion app. Silicon to phone, evaluation kit to production.

**Client:** A US medical-wearable / health-tech company *(name withheld — NDA)*
**Stack:** nRF5340 (nRF Connect SDK / Zephyr, dual-core App+Net), BLE, USB, MCUboot, 1 Gb NAND, C#/.NET MAUI, GitHub Actions CI/CD
**Role:** Embedded developer (firmware) + mobile developer (companion app), at Croxel Inc
**Timeline:** 2022 – 2026 — the longest engagement of my Croxel tenure

## The product

A wristband worn by **patients in clinical studies** that continuously captures physiological data and hands it to a **data-science team**, who process it to identify underlying health issues. Because the data drives clinical conclusions, the firmware's job isn't just "read sensors" — it's to capture data that is **time-accurate, integrity-checked, and complete**, on a device that runs for a month on a charge and survives FCC certification and real-world production.

---

## Part 1 — Wearable firmware (nRF5340)

### Data capture & correctness
- **Multi-sensor acquisition:** IMU, accelerometer, magnetometer, barometer, and **PPG** (for blood pressure / SpO₂), buffered to **1 Gb NAND** flash.
- **Timing synchronization** — treated as first-class, because misaligned timestamps corrupt the data-science analysis downstream. Getting time right across the system was one of the critical engineering problems.
- **Data-integrity checks** end to end, so corrupted or partial records never masquerade as clinical data.

### Dual-core architecture & connectivity
- **Dual-core nRF5340 (Application + Network core)** with inter-core communication (IPC), distributing peripherals and workload across the two cores.
- **BLE throughput raised from ~300 kbps to ~1.2 Mbps — roughly 4×** — so a month of buffered sensor data offloads in reasonable time.
- **Vendor-specific USB protocol** for high-rate wired data paths.

### Production-grade robustness
- **MCUboot dual-bank bootloader** for safe OTA updates.
- **Coredump** capture to diagnose in-field crashes — post-mortem debugging on devices already in patients' hands.
- **Direct Test Mode (DTM)** firmware for **FCC certification** of the radio.
- **~30-day battery life** through low-power design across the whole system.

### Engineering discipline
- **Full test coverage with a CI/CD pipeline** built specifically to keep production bugs out — this is the test-driven, automated-release discipline applied to a regulated medical device.
- **Full production lifecycle:** firmware carried across **evaluation kits → development kits → production kits**, with the code-management and release discipline that a shipping medical product demands.

---

## Part 2 — Companion mobile app (C# / .NET MAUI)

- **Migrated the production companion app from Xamarin to .NET MAUI** — a full framework migration of a shipping app, not a greenfield rewrite.
- **Raised BLE throughput** on the app side to match the firmware improvements — both ends of the link had to cooperate to hit the higher rate.
- **Implemented and tested background sync**, so the wristband's data offloads reliably even when the app isn't in the foreground.

---

## The result

- A shipping, FCC-certified clinical wearable with a month-long battery, 4× faster data offload, and the production-lifecycle rigor (test coverage, CI/CD, coredump diagnostics) that regulated medical hardware requires — plus the cross-platform app patients use every day.
- What this demonstrates: **end-to-end medical-device product engineering** — multi-sensor low-power firmware, dual-core architecture, BLE/USB performance work, FCC certification, MCUboot/OTA, and a full CI/CD + test regime — *and* cross-platform mobile development (C#/MAUI) on the same product. Very few engineers cover this entire span on one device.

