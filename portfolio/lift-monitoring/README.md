# Lift Monitoring System — CircuitPython → Zephyr, with a Data-Driven Algorithm Simulation Framework

**Outcome in one line:** Took an elevator-monitoring product from **CircuitPython prototype to production Zephyr firmware** (STM32L0, NB-IoT) and built a simulation harness that replays real trip data through the shipping C algorithm — **cutting months off device testing**.

**Client:** A US lift/elevator analytics company *(name withheld — NDA)*
**Stack:** STM32L0 (Zephyr RTOS), accelerometer, barometer, SD card, NB-IoT cellular (Blues Notecard), C, Python (FFI simulation harness)
**Role:** Embedded developer — productionization, algorithm, and test framework (at Croxel Inc)
**Timeline:** 2023 – 2024

## The problem

The client had a working **floor/trip-detection algorithm** for monitoring elevators — but it lived in **CircuitPython**, a prototyping environment, not production firmware. Two things had to happen: move it onto a real, low-power, battery-powered production platform, and — the harder part — **validate the detection algorithm** without burning months physically riding elevators to test every change.

## What I built

### Productionization
- **Migrated the algorithm from CircuitPython to production Zephyr firmware** on an **STM32L0**, folding in production lessons (coredump diagnostics, robust data handling, release discipline) from earlier projects.
- **Low-power engineering** throughout — the device is battery-powered, so the firmware and duty-cycling are optimized for long battery life.
- **Sensing & connectivity:** accelerometer + barometer for motion/altitude, **SD-card** logging for local data, and an **NB-IoT cellular data card (Blues Notecard)** for backhaul.

### The Algorithm Simulation Framework (ASF)
The centerpiece — an **algorithm-development and optimization harness**, distinct from a SIL test:
- It **compiles the real production C algorithm** — not a Python reimplementation — so what's tuned is exactly what ships.
- It drives that compiled algorithm from **Python via FFI**, feeding it **datasets recorded from many real sample trips**.
- Engineers could then **replay hundreds of real elevator trips through the actual detection code in seconds** on a desktop, **iterating on the algorithm and re-running until floor/trip detection was satisfactory**.

> Not a SIL test (which asserts a known-correct output) — an **optimization loop**: replay real data, measure detection quality, adjust the algorithm, repeat.

## The result

- **Device-testing cycles cut by months** — algorithm changes were validated against recorded reality instantly instead of via slow physical field testing.
- **Shipped** the product with an optimized floor/trip-detection algorithm.
- What this demonstrates: **prototype-to-production migration, low-power cellular IoT firmware, and — above all — algorithm-development infrastructure.** The ASF (iterate the real compiled algorithm against recorded field data) is exactly the kind of harness that turns "tune it on the device and hope" into "optimized against hundreds of real trips before it ever ships."

