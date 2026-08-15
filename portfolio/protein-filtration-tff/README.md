# Protein Filtration Control Library — Bioprocessing TFF System

**Outcome in one line:** Built the Windows control library behind a **tangential-flow-filtration (TFF)** system for a US bioprocessing-equipment manufacturer — real-time monitoring and control of 50+ parameters, with a PID rewrite that reached steady state **3× faster** at **2× lower error**. The same instrument line was later used in COVID-19 testing.

**Client:** A US-based bioprocessing-equipment manufacturer *(name withheld — under NDA)*
**Stack:** Java (multi-threaded library), Windows, PID control, real-time instrument comms
**Role:** Firmware/software developer — control library, API, control algorithm (at Lattice Innovations)
**Timeline:** 2019

## The problem

Tangential-flow filtration (TFF) concentrates and purifies biologics — proteins, vaccines, therapeutics. The system runs **filtration, diafiltration, and intermediate steps as a profiled process**, not a single fixed operation, while continuously watching flow and pressure at both input and output. The instrument needed a control layer that the product's backend and frontend could drive: monitor every parameter in real time, and control the machine safely through each stage.

## What I built

- **A multi-threaded Java control library for Windows** that talks to the instrument and monitors/controls **50+ system parameters** in real time — the engine the rest of the product's UI is built on.
- **A clean API surface** exposed to the front end, so operators drive the machine through a GUI without touching the low-level instrument protocol.
- **Process profiling** for filtration / diafiltration (and intermediate distillation-style steps), sequencing the stages that turn raw fluid into a purified product.
- **Continuous flow and pressure monitoring** at input and output — the feedback that keeps the process inside safe, correct operating bounds.
- **An advanced PID control algorithm** I proposed and implemented to replace the original control loop: **steady state reached 3× faster** with **steady-state error cut 2×**.

## The result

- Delivered the control library that the TFF product relied on for monitoring and control.
- Measurable control improvement: **3× faster** steady state, **2× lower** steady-state error versus the original algorithm.
- The same instrument line was later used in **COVID-19 testing** — a meaningful place for the work to end up.
- What this demonstrates: **real-time control-software engineering for a medical/bioprocess client, multi-threaded systems design, and control-algorithm improvement with measured results.**

