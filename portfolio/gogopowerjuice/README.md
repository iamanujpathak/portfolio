# GoGoPowerJuice — Power-Bank Rental System (Charger Hardware + Full Software Stack)

**Outcome in one line:** Built both halves of **GoGoPowerJuice's** power-bank rental product — the **multi-channel USB-C Power Delivery charging hardware** (5/10-channel from a single 180 W supply) and the **complete software system** (vending kiosk, backend, frontend, rental app) — everything but the vending-machine enclosure.

**Client:** GoGoPowerJuice *(public freelance engagement — visible on my Upwork / Freelancer profiles)*
**Stack:** Cypress (Infineon) USB-C PD controller ICs, PCB design, USB-C Power Delivery, Flutter, backend + frontend web, mobile rental app
**Role:** Freelance hardware + full-stack developer
**Timeline:** 2022 – Present (ongoing, multi-stage) · via Freelancer & Upwork

---

## Part 1 — Multi-power-bank charger hardware

The physical heart of a rental station: a charger that keeps a rack of power banks topped up and ready to rent.

- **Multi-channel USB-C Power Delivery chargers** built around **Cypress (Infineon) PD controller ICs**, in **5-channel and 10-channel** variants.
- **Single 180 W power adapter** feeding every channel — so the design has to **budget and allocate power intelligently across channels** rather than assume unlimited supply, negotiating USB-C PD per port within a fixed shared power envelope.
- PCB design for the charging board.

## Part 2 — Battery-vending software system

Effectively the entire product software, minus the vending-machine hardware/PCB:

- **A Flutter vending kiosk app** — the on-station interface where customers rent and return power banks.
- **Backend** services powering the system (rentals, inventory, billing/state).
- **Frontend** for management/operations.
- **A user rental mobile app** — the customer-facing app to find, rent, and return power banks.

Together this is a **complete rent-a-charger system**: a customer walks up (or opens the app), rents a charged bank, and returns it — with the backend tracking every unit and the kiosk hardware dispensing and recharging.

## The result

- Delivered both the **power hardware** and the **full software stack** for a shared power-bank rental business as a freelance engagement.
- **In market today:** charging docks and kiosks deployed with **12+ retail and hospitality partners** (Florida, US), and the customer rental app is **live on the App Store and Google Play**.
- What this demonstrates: **USB-C Power Delivery hardware design (multi-channel power budgeting on real PD silicon)** *and* **full-stack product software (kiosk + backend + frontend + mobile app)** — the rare hardware-plus-software span, delivered independently as a contractor.

## Client feedback

> *"It was an amazing experience working with BIII TECH LLP. Goes above and beyond to get the project completed. Communication was concise and prompt, and there was a sense of accountability to help achieve the goals of the project. This was the first time working with BIII TECH LLP, and it won't be my last. Highly recommend!"*
> — 5.0★ [Freelancer review ↗](https://www.freelancer.in/u/iamanujpathak) on the first USB-C PD charger board (2022)

> *"Amazing work with dedication to detail to make the project a success. I've worked multiple projects and very happy with the work and outcome. Would highly recommend and will continue to work on future projects and endeavors."*
> — 5.0★ [Upwork review ↗](https://www.upwork.com/freelancers/~01a418fb5c16816290) on Stage 1: the 10-slot charging dock (2023)

"It won't be my last" held up: the engagement has run through multiple stages across both platforms and continues today — currently **Stage 3 (frontend/backend app), 355+ hours logged**.

## Links

- **Live product:** [gogopowerjuice.com ↗](https://gogopowerjuice.com/) — the docks, kiosks, and rental system in commercial operation
- **The rental app I built, live on both stores:** [App Store ↗](https://apps.apple.com/in/app/gogopowerjuice/id6472820548) · [Google Play (developer page) ↗](https://play.google.com/store/apps/developer?id=GoGoPowerJuice+Inc.)

