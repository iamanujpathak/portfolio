# Connected Access Control Board — STM32F4 + ESP32 Dual-Processor

**Outcome in one line:** Designed a cloud-connected single-door access controller as a **dual-processor system** — an STM32F4 host owning the security-critical real-time logic, an ESP32 handling WiFi/BLE — so the radio never touches the access path. MQTT cloud control, with **OTA over both MQTT (remote) and BLE (on-site)**.

**Stack:** STM32F4 (host), ESP32 (connectivity), Embedded C, WiFi, BLE, MQTT, dual-path OTA
**Role:** Research & Solution Architect — architecture and firmware (at IoTech Designs)
**Timeline:** 2019 – 2021

## The problem

The earlier [multi-credential access controller](../access-control-system/README.md) scaled across many doors over RS485, but some installations need the opposite: a **single self-contained connected door**, no wired controller network — just the door, the cloud, and a phone. That means putting real-time access-control logic *and* modern wireless connectivity on one board without letting the radio stack interfere with the security-critical timing.

## What I built

- **A dual-processor (multi-processor) architecture:** an **STM32F4 host** owning the access-control logic and real-time I/O, with an **ESP32 as a dedicated connectivity coprocessor** for WiFi and BLE. Separating the two keeps the radio's workload off the security-critical path.
- **The same access-control feature set** as the multi-door system — credential handling, access logic, tamper detection — scoped to single-board control.
- **MQTT connectivity** for cloud-based control and monitoring over WiFi.
- **Dual-path OTA:** firmware updates delivered over **both MQTT (remote/cloud) and BLE (local/on-site)** — so a device can be updated from the field or from a phone standing next to it.

## The result

- A connected, self-contained access-control board complementing the networked multi-door platform — same security features, cloud-native deployment model.
- What this demonstrates: **multi-processor system architecture, host/coprocessor partitioning, cloud (MQTT) and BLE connectivity, and robust multi-path OTA design** on security-critical hardware.

## Related

- Sibling product to the **[multi-credential access control system](../access-control-system/README.md)** (SAMD21, RS485-networked multi-door). Same domain, different deployment model.
