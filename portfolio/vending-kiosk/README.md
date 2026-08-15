# Connected Vending Kiosk — Flutter UI on Raspberry Pi + Cloud Sync

**Outcome in one line:** Architected and built a cloud-connected vending-machine kiosk on Raspberry Pi — a Flutter UI running full-screen in locked single-app kiosk mode, backed by a native peripheral-control layer that drives the machine's hardware and keeps inventory in sync with the cloud.

**Client:** An intelligent-vending company *(name withheld — NDA)*
**Stack:** Raspberry Pi (Linux), Flutter (kiosk UI), C + Python (peripheral/control layer), WebSocket IPC, GDBus/BLE, cloud REST, bash
**Role:** Architect & developer — full kiosk stack (at IoTech Designs)
**Timeline:** 2019 – 2021

## The problem

A vending machine needs a kiosk that feels as polished as a phone app, but that UI also has to reach down and physically run the machine — motors, refrigeration, heater, drop/weight sensors — reliably and safely. This one added a twist: it had to be **connected**, staying in sync with a cloud backend for inventory rather than running as an isolated island.

## What I built

- **A Flutter kiosk UI on Raspberry Pi**, booting full-screen into locked **single-app kiosk mode** — install and autoboot handled by bash scripts that lock the device to the one app, so it comes up as an appliance, not a desktop.
- **UI that evolved from PoC to production:** the PoC ran Flutter in **Chromium kiosk mode** over **WebSocket IPC**; production moved to **native Flutter** on the Pi, dropping the browser overhead.
- **A native peripheral-control layer in C and Python** that drives the machine's subsystems — dispense motors, refrigeration, heater, and drop/weight sensors — exposed to the UI through clean peripheral APIs.
- **BLE peripheral support** on Raspberry Pi (and Pine A64) via **GDBus**, for local device interaction.
- **Cloud connectivity** closing the loop: fetch live inventory from the cloud, let the customer build a cart, dispense the items, then **write the updated inventory back to the cloud** — keeping every machine continuously in sync.

## The result

- A complete connected-vending kiosk: app-grade UI, robust hardware control, and cloud-synced inventory on affordable SBC hardware.
- What this demonstrates: **full-stack embedded-Linux product development** — UI, native hardware control, IPC, BLE, and cloud integration — plus the Linux/kiosk system engineering (single-app lockdown, autoboot) that turns a Raspberry Pi into a shippable appliance.

