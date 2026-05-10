<div align="center">

# SolWear

### A Solana hardware wallet you wear.

**Transparent crypto smartwatch for tap-to-pay Solana flows, built from firmware to mobile relay.**

[![Solana](https://img.shields.io/badge/chain-Solana-9945FF?style=for-the-badge&logo=solana&logoColor=white)](https://solana.com)
[![Hardware](https://img.shields.io/badge/hardware-ESP32--S3-14F195?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/status-Frontier%20Prototype-111827?style=for-the-badge)]()

[Website](https://solwear.tech) · [X](https://x.com/SolWear_) · [Instagram](https://instagram.com/solwear.watch) · [TikTok](https://tiktok.com/@solwear)

</div>

---

## What we are building

Hardware wallets are still mostly single-purpose devices that live in a drawer. SolWear brings wallet custody into a smartwatch form factor: a device that can show account state, handle approvals on its own screen, coordinate NFC signing flows, and stay with the user throughout the day.

The current prototype combines **SolWearOS** firmware on an ESP32-S3 Mini, an Android companion app for NFC pairing and Solana transaction relay, a desktop service tool for flashing and diagnostics, and a web presence for the project.

## Prototype stack

| Repository | Purpose | Stack |
| --- | --- | --- |
| [solwear](https://github.com/SolWear/solwear) | Public Frontier Hackathon bundle: firmware, mobile app, service tool, website, and profile material | ESP-IDF, Kotlin, Python, Next.js |
| [solwear_os](https://github.com/SolWear/solwear_os) | Embedded smartwatch firmware with wallet, NFC, UI, games, storage, and hardware drivers | C, ESP-IDF, ESP32-S3 |
| [solwear_mobile](https://github.com/SolWear/solwear_mobile) | Android companion for NFC pairing, wallet preview, signing requests, and transaction relay | Kotlin, Jetpack Compose |
| [solwear_service_tool](https://github.com/SolWear/solwear_service_tool) | Desktop utility for serial inspection, status dashboards, settings, and firmware flashing | Python, Tkinter |
| [solwear_site](https://github.com/SolWear/solwear_site) | Project website and supporting product pages | Next.js, React, Tailwind |

## Current prototype

- **On-device wallet flow**: local wallet creation/import, passphrase-protected seed storage, and approval UI on the wearable.
- **NFC signing surface**: PN532-based pairing and signing session flow between the watch and the Android app.
- **Android transaction relay**: the phone prepares Solana sends, requests a signature from the watch, then broadcasts the signed payload through Solana RPC.
- **Smartwatch experience**: watchface, settings, transaction, stats, battery status, games, and system UI built for the hardware demo.
- **Service tooling**: live serial console, device status dashboard, settings workflows, and one-click firmware flashing.

## Prototype hardware

| Component | Part |
| --- | --- |
| MCU | ESP32-S3 Mini |
| Display | ST7789 240 x 240 IPS over SPI |
| NFC | PN532 over I2C |
| Power | TP4056 charger with 350 mAh LiPo |
| Input | Four active-low tactile buttons |
| Storage | NVS for wallet material, SPIFFS for receipts and game state |

## Why it matters

SolWear is exploring what everyday crypto payments can feel like when the wallet is not a browser extension or a USB stick, but a small piece of hardware on the wrist. The goal is a fast NFC payment loop for Solana where private keys stay on the wearable and the phone acts as a thin relay.

---

<div align="center">

**[See the full project](https://github.com/SolWear/solwear)**

<sub>More secure. More comfortable. More Solana.</sub>

</div>
