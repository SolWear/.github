<div align="center">

# SolWear

### *Your Solana wallet on your wrist.*

**A portable, light, hardware wallet for crypto — built into a smartwatch.**

[![Solana](https://img.shields.io/badge/chain-Solana-9945FF?style=for-the-badge&logo=solana&logoColor=white)](https://solana.com)
[![RP2040](https://img.shields.io/badge/MCU-RP2040-blueviolet?style=for-the-badge)]()
[![PlatformIO](https://img.shields.io/badge/build-PlatformIO-orange?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/status-Hackathon%20Demo-14F195?style=for-the-badge)]()

</div>

---

## What we're building

Hardware wallets today are **single-purpose USB sticks** you forget in a drawer. We think the wallet you actually use should be the one you actually wear.

**SolWear** is a smartwatch that's also a Solana hardware wallet. It signs transactions, taps NFC payment tags, runs an app launcher, counts your steps, and never leaves your wrist. Built on a Waveshare RP2040-Touch-LCD-1.69 with our own from-scratch operating system.

| | |
|---|---|
| One purpose | Smartwatch + wallet + fitness + NFC |
| Lives in a drawer | Lives on your wrist |
| Plug into a computer | Tap a phone, tap a terminal |
| You forget about it | You wear it 24/7 |

## Our repositories

| | |
|---|---|
| **[solwear](https://github.com/SolWear/solwear)** | The main project — hackathon showcase, prototype, landing page |
| **[solwear_os](https://github.com/SolWear/solwear_os)** | Smartwatch firmware: HAL, kernel, UI, eight apps, Solana wallet |
| **[solwear_service_tool](https://github.com/SolWear/solwear_service_tool)** | Desktop debugger: live console, status dashboard, UF2 flasher |

## Hardware

- **RP2040** · 264 KB SRAM · 16 MB flash
- **ST7789V2** 1.69" 240×280 IPS touchscreen
- **CST816S** capacitive touch
- **QMI8658** 6-axis IMU
- **PN532** NFC reader *(off by default)*
- **1200 mAh** LiPo battery
- Passive piezo audio

## SolWearOS highlights

- Custom from-scratch OS — **12 KB RAM · 196 KB flash**
- Square-icon app launcher with eight apps
- Lazy NFC initialization for security & power
- Animated charging screen, live battery & system stats
- Procedural icons & wallpapers (zero flash cost)
- Three watch faces · LittleFS persistence · 30 fps event loop

## Built for

The **Frontier Hackathon** — by the SolWear team.
Hardware, firmware, desktop tools, and branding — all in-house.

---

<div align="center">

**[See the full project →](https://github.com/SolWear/solwear)**

<sub>Portable. Light. Always with you. The Solana wallet you actually wear.</sub>

</div>
