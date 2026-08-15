# Blood Slide Heater — Precision Thermal Profiling for Medical Labs

**Outcome in one line:** Delivered a precision blood-slide preparation instrument in **3 months** — hand-tuned PID thermal control with programmable multi-step temperature profiles — now **in production use at local labs**.

**Client:** A medical-equipment client *(name withheld — NDA)*
**Stack:** ATmega2560 (Arduino Mega), Embedded C, PID control, custom power electronics, HMI GUI, USB data logging
**Role:** Firmware developer — control algorithm, electronics, GUI, logging (at Lattice Innovations)
**Timeline:** 2019, delivered within 3 months

## The problem

Preparing blood slides for testing isn't "heat to X degrees and hold." Samples must follow a **thermal profile** — a sequence of set temperatures, each held for a set duration — and precision matters: overshoot can damage a sample, and drift ruins repeatability between tests.

## What I built

- **Custom electronics** for high-frequency switching of the 12 V heat bead, paired with a fan for active cool-down — giving the control loop authority in *both* directions instead of waiting on passive cooling.
- **A PID control loop driving heater and fan together**, with coefficients tuned empirically: collect response data, adjust, re-run — iterating until overshoot, undershoot, and steady-state error were minimized — tuned against the real thermal mass, not a paper model.
- **A thermal profiling engine** — the operator defines an array of (temperature, duration) steps and the instrument executes the full preparation sequence unattended.
- **A state machine** managing profiles, safety, and user interaction, fronted by an **HMI-based GUI**.
- **Compliance logging:** every run's temperature trace is logged to a file on USB — a per-run compliance record for the lab.

## The result

- Delivered within the **3-month** target.
- **In production use at local labs** for blood-sample testing.
- What this demonstrates: **control-systems engineering on real hardware, medical-instrument delivery discipline, and full-stack instrument development** — power electronics to GUI.

