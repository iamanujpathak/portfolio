# A21 — Code-Protected Binary Firmware Library with a Syscall-Style ABI

**Outcome in one line:** Turned a tightly coupled access-control codebase into a reusable, **code-protected binary firmware library** with an OS-like syscall ABI — so one physical board ships as multiple products, each just a simple business-logic app running on the shared, precompiled library.

**Stack:** STM32F415 (ARM Cortex-M4), Embedded C, SVC / vector-table ABI, two-stage bootloader, custom HAL
**Role:** Research & Solution Architect — system architecture & core library (at IoTech Designs)
**Timeline:** 2019 – 2021

## The problem

In access control, ~80% of the firmware is the same from board to board — readers, I/O handling, access logic. But in the client's codebase it was all **cross-linked**, so the reusable majority couldn't be reused: every new product meant reworking shared code, and the *same hardware could not be sold as different products* without a rewrite.

There was a second, harder constraint: **code protection.** The shared IP could not ship as source — not even as a static library, which still links into the customer's app where it can be picked apart. The reusable core had to be genuinely sealed.

## What I designed

I split the reusable core out as a **standalone firmware library distributed as a precompiled binary** placed at a fixed memory location — never source, never a linkable object. The application and the library are separate binaries that meet only through a stable interface:

- **Two-stage boot:** a primary bootloader loads the library; the library, in turn, hands off to and starts the application.
- **A syscall-style ABI.** The library exposes every service — hardware peripherals (GPIO, I2C, SPI, ADC) and higher-level logical modules (inputs, outputs, card readers) — through a **vector table** at a known location, the way an OS exposes a syscall table. The app calls in through a **software interrupt (SVC)**; arguments are passed and **return codes delivered via stack-frame manipulation**. The result is a binary interface that stays stable without any linking between app and library.
- **The library owns and arbitrates all resources** — it manages peripheral access and resolves conflicts centrally, so two logical modules can't collide over the same hardware.
- **The application is deliberately trivial** — Arduino-simple C, concerned only with business logic, calling library APIs. No peripheral wrangling, no conflict handling, no boot logic.
- **A HAL wrapper layer** beneath the library, so the underlying MCU can be swapped in future without touching either the library's or the application's logic.
- Event-based throughout — no busy-wait delays — with layered architecture and channel support.

## The result

- **Shipped in production.** The platform is used in commercial access-control products in the field — this is a deployed architecture, not a prototype.
- **One board → multiple products.** Because an app is just business logic jumping into the shared library, the same board runs different apps and ships as different products — with **zero rework of the protected core.** A new product becomes "write a small business-logic app."
- **Client IP sealed.** The shared code leaves only as a precompiled binary behind a stable ABI — no source, no relinkable object.
- **Future-proofed** against MCU changes via the HAL layer.
- What this demonstrates: **OS-level architecture on bare metal** (syscall ABI via SVC + vector table + stack-frame marshalling), **binary ABI/interface design, central resource arbitration, a code-protection strategy, and portability engineering** — the kind of foundational design a whole product line is then built on.

