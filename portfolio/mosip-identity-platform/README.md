# MOSIP Identity-Management Platform (PoC) — Biometrics with PKI Trust

**Outcome in one line:** Built a proof-of-concept identity-management stack on the open-source **MOSIP** standard — the platform behind national-ID programs, comparable to India's UIDAI/Aadhaar — with **biometric capture (fingerprint, iris, face) on a Raspberry Pi 4 device server** and **certificate-chain trust** securing identity at every stage.

**Engagement:** Techno Brains Group (full-time consultancy via Eureka Solutions)
**Stack:** Java Spring Boot, Java + C (device server), Raspberry Pi 4, MOSIP compliance, PKI / certificate chains, biometric capture devices
**Role:** Senior embedded developer — device server, services, and backend
**Timeline:** November 2021 – April 2022

## The problem

National-scale identity systems can't just *capture* biometrics — every capture device must be **trusted**, and every identity record must be **verifiable** as it moves through enrollment, storage, and authentication. **MOSIP** (Modular Open Source Identity Platform) is the open-source standard several countries build national ID on, and it enforces exactly this: certified devices, signed data, and authority-verified trust chains. The goal was a working MOSIP-compliant stack proving the whole pipeline.

## What I built

- **A MOSIP-compliant device server on Raspberry Pi 4 (Java + C)** capturing user identity biometrics — **fingerprint, iris, and face**.
- **Certificate-chain and authority verification** throughout: identity data is stored, loaded, and verified against the PKI trust chain at each stage of the pipeline, so no unsigned device or tampered record passes.
- **A management server in Java Spring Boot** — the backend of the identity system.
- **A background desktop service** (Java) for device monitoring, and a **desktop UI client** driving the device server's and desktop service's APIs.

## The result

- A working PoC demonstrating the full MOSIP identity pipeline — trusted capture on real hardware through PKI-verified storage and verification to the management backend.
- What this demonstrates: **security engineering (PKI, certificate chains, device trust), standards compliance (MOSIP), biometric-device integration, and Java/Spring Boot backend development** — proof the skill set extends from bare-metal firmware up through secure backend systems.
