# Gyani — No-Code Robotics Learning Platform

**Outcome in one line:** Founded an ed-tech startup and single-handedly built the entire product — custom PCB, bytecode-interpreting embedded OS, flowchart-to-bytecode compiler, desktop + Android apps, OTA bootloader. Completed and taken beyond PoC; the company wound down on marketing, not engineering.

**Product naming:** *Gyani* ("knowledgeable") was the project; the device shipped as **Gyan-Yantra**, the application as **Gyan-Matra**.

**Stack:** nRF51822 (nRF5 SDK 12), FreeRTOS, Embedded C, KiCad, JavaFX, Kotlin/Java (Android), BLE + USB-UART
**Role:** Co-Founder — sole hardware, firmware, and software engineer (Bhawna Infinity Tech)
**Timeline:** mid-2016 – early 2018

## The problem

Teaching kids embedded programming normally means toolchains, compilers, and firmware flashing — a wall of friction before anything blinks. The goal: let children program real hardware by drawing a **flowchart with conditional paths**, and have it run on the board *instantly* — no toolchain, no reflashing, no waiting.

## What I built

- **A Java-like bytecode interpreter in Embedded C on FreeRTOS** (nRF51822, nRF5 SDK) — a small embedded OS that receives bytecode programs and executes them **on the fly from RAM**. Reprogramming the board takes seconds, with zero flash-wear cycles for every student iteration.
- **A custom bytecode instruction set** designed to fit embedded constraints while covering peripheral initialization and control — the contract between the kids' flowcharts and the silicon.
- **A flowchart IDE, twice:** JavaFX desktop application and Kotlin/Java Android application built on a **shared Java core** — students draw the logic, the shared compiler translates the flowchart (branches included) into bytecode.
- **A custom transfer protocol over BLE and USB-UART** carrying programs from the IDE to the board.
- **A dual-bank bootloader** supporting OTA firmware updates over both BLE and USB-UART, with cloning protection for the platform firmware itself.
- **The hardware:** board and module PCBs designed in KiCad, fabricated, assembled, and tested.

## The result

- The platform was **completed and moved beyond proof-of-concept** — hardware, firmware, and both apps working end to end.
- The startup ultimately failed at **marketing and distribution** — an honest lesson in why product ≠ business, and the experience behind how I scope client work today.
- What this demonstrates: **whole-product ownership** — from schematic to silicon to compiler to app store, one engineer.

## Demo videos

1. **[Gyani 01 — Walkthrough](https://www.youtube.com/watch?v=RQ05I6xJ4js)** — platform overview
2. **[Gyani 02 — Blink a LED](https://www.youtube.com/watch?v=FUhqrbocwGk)** — the embedded "hello world," from flowchart to running hardware
3. **[Gyani 03 — Remote Control Car](https://www.youtube.com/watch?v=h7ZZa9d3q-w)** — a full robot built and programmed on the platform

