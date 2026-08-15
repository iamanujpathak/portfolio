# BLE Beacon Mesh Home Automation

**Outcome in one line:** Designed a complete retrofit home-automation system — custom mains-side hardware, a custom BLE beacon mesh protocol, and an Android app — that ran my own house for **2+ years of continuous operation**. Stopped before mass production by funding, not engineering.

**Stack:** nRF51822 (nRF5 SDK 12), Embedded C, custom BLE beacon mesh, Android, KiCad (PCB), FreeCAD (enclosure)
**Role:** Solo designer — hardware, enclosure, firmware, protocol, and app
**Timeline:** 2018 – early 2019 (after Gyani, before first full-time role); field-tested at home for 2+ years, into the COVID period

## The problem

Smart-home products mostly assume new wiring, a WiFi hub, or a cloud subscription. The goal here was a **retrofit** system for traditional Indian modular switchboards: no rewiring, no hub, no cloud — and a bill of materials low enough for whole-house deployment to make sense.

## What I built

- **Hardware in the switchboard's own form factor:** a 5×5 cm main board and 2.5×5 cm switch modules sized to drop into standard modular household switch plates.
- **Cost-engineered architecture:** the main board carries the controller, a custom AC-DC supply, EEPROM, and solid-state switching — and **one main board drives up to 16 switch boards**, so the expensive parts are bought once per room cluster, not once per switch. That single decision collapses the whole-house BOM.
- **A custom BLE beacon mesh** — designed from scratch on nRF51822, letting every board in the house relay status and commands with no hub and no pairing ceremony.
- **An Android app** that joins the beacon mesh directly, showing live switch status across the house and controlling any switch.
- **PCBs in KiCad, enclosures in FreeCAD** — the modules had to fit standard modular switch plates mechanically, not just electrically.

## The result

- PoC completed and **deployed in my own home, where it ran for more than 2 years** of daily use.
- One hardware failure in that time: the AC-DC stage fused after a short in the home's power inverter — an external fault, not a design flaw.
- The project ended in a cash crunch before mass production.
- What this demonstrates: **mains-adjacent hardware design, cost engineering for BOM-sensitive products, custom wireless protocol design, and multi-year field reliability.**

