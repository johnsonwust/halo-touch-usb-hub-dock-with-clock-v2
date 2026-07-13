# HALO TOUCH USB Hub Dock with Clock V2

English documentation repository for the **HALO TOUCH USB Hub Dock with Clock V2**, a multifunction desktop USB hub and display dock sold by **innoelement / Johnson**.

[Product Page on Tindie](https://www.tindie.com/products/johnson/halo-touch-usb-hub-dock-with-clock-v2/)
[Original Chinese Manual](http://pressf5.run/?p=227)
[Chinese Companion README](./README.zh-CN.md)
[Contributing Guide](./CONTRIBUTING.md)
[License](./LICENSE)

## Overview

HALO TOUCH V2 is a compact desktop dock that combines a USB 2.0 hub, round IPS display, touch interface, rotary control, TF card storage, clock functions, media playback, and several utility modes for PC and desk use.

Based on the official product listing and the original Chinese instructions, the device is positioned as a DIY desktop companion rather than a mass-market certified peripheral. It is designed for users who want a visually distinctive desk hub with monitoring, media, and control functions in one enclosure.

## Main Features

- Round 360 x 360 IPS display
- Touch interaction and rotary knob control
- USB 2.0 hub with 2 x USB-A and 1 x USB-C downstream ports
- USB-C upstream connection to the host computer
- USB-C PD auxiliary power input for higher-load scenarios
- TF / microSD card reader for local assets and system files
- Per-port voltage, current, and power monitoring
- Pomodoro timer with haptic feedback
- Music box / MP3 playback mode
- Photo frame and MJPEG animation playback
- Microphone audio spectrum visualization
- AIDA64 system-monitor display mode
- Surface Dial style desktop control support on Windows 10 or later
- OTA firmware update support
- 100 Mbps Ethernet port for basic network use

## Hardware Layout

The original manual describes the following interfaces and controls:

| Item | Description |
| --- | --- |
| `USB-PC` | USB 2.0 Type-C upstream port to the computer |
| `PWR-PD` | USB Type-C PD power input |
| `USB1` / `USB2` | USB 2.0 Type-A downstream ports |
| `USB3` | USB 2.0 Type-C downstream port, shared with flashing/programming use |
| `TF` | microSD / TF card slot |
| `LAN` | 100 Mbps Ethernet |
| Knob | Rotary input for timing, control, and mode interaction |
| Touch display | Main UI for status pages and interaction |

## Power Modes

HALO TOUCH V2 supports two main power arrangements:

### 1. PC-powered mode

This is the default mode. Connect the `USB-PC` port to a computer and allow the computer USB connection to provide power.

### 2. PD-assisted mode

If the connected peripherals draw more current than the host computer port can comfortably supply, connect a PD charger to `PWR-PD`.

### Important power note

The original instructions explicitly warn **not** to connect a USB-C power adapter directly into the `USB-PC` port as a replacement for the host connection. Use the dedicated `PWR-PD` port for external power input.

## Basic Setup

1. Connect `USB-PC` to the computer.
2. If additional power is needed, connect a PD charger to `PWR-PD`.
3. Insert the supplied TF card, or prepare a replacement TF card as described below.
4. Connect your peripherals to the downstream USB ports.
5. Power on the device and confirm the display boots normally.
6. Enter the relevant mode for clock display, hub monitoring, media playback, or AIDA64 display.

## TF Card Requirements

The original instructions say the device is normally shipped with a preconfigured 4 GB TF card containing required system files.

If you replace the card:

- Use a TF / microSD card of **32 GB or smaller**
- Format it as **FAT32**
- Keep the required system folders intact

Expected directory structure:

| Folder | Purpose |
| --- | --- |
| `fonts` | Font resources |
| `mjpeg` | MJPEG animation files |
| `music` | MP3 files |
| `night7` | System assets including alarm sound |
| `pic` | JPG image files |
| `aida64` | AIDA64-related assets |

Do not delete required system files from the shipped TF card unless you have a verified backup.

## Wi-Fi Configuration

According to the original manual:

- Only **2.4 GHz Wi-Fi** is supported
- Default hotspot SSID: `My-Ap`
- Default hotspot password: `12345678`
- Local configuration page: `192.168.4.1`

The manual also mentions a file-based Wi-Fi configuration method using `wifi.txt`.

## Recommended USB Hub Usage

The original guide recommends a layout similar to:

- `USB-PC` -> computer
- hardware switch -> PC mode
- `USB1` -> keyboard
- `USB2` -> mouse
- `USB3` -> additional peripheral

The integrated 100 Mbps Ethernet port is described as suitable for basic or emergency use rather than high-performance networking.

## Operating Modes

## USB Monitor Mode

The device can display per-port electrical data including voltage, current, and power. The Chinese manual states that long-press gestures in the upper or lower touch areas can be used for port power switching and related controls.

## Pomodoro Timer

- Default timer length: 25 minutes
- The knob is used to adjust the duration
- The device can vibrate once per second during countdown
- Alarm audio uses `night7/alarm.mp3`

## AIDA64 PC Monitor Mode

HALO TOUCH V2 can be used as a round hardware-monitor display for a Windows PC with AIDA64.

The original Chinese instructions reference:

- AIDA64 setup video: [Bilibili tutorial](https://www.bilibili.com/video/BV1A64y1w723)

The manual mentions:

- default port `80`
- remote sensor setup around `1280 x 800`
- the device-side `aida64` folder for related assets

## Music Box Mode

- Place MP3 files in the `music` folder
- The knob can be used to "wind up" or control playback duration

## Photo Frame and Animation Mode

- Put MJPEG files into `mjpeg`
- Put JPG image files into `pic`

This allows HALO TOUCH V2 to act as a compact animated desk display.

## Audio Spectrum Mode

The device includes a microphone-driven visualization mode that reacts to nearby sound or music.

## Surface Dial Support

The original manual says Surface Dial style support is available on firmware `1.3.0` or later, and is intended for Windows 10 or newer. A long press on the screen is used to invoke the control behavior.

## OTA Update

The original instructions indicate that firmware updates can be checked from the on-device system menu:

`Settings -> System -> Other -> Check for Updates`

## Safety Notes

- Keep the device away from moisture and wet environments
- Do not use damaged cables or visibly damaged connectors
- Avoid placing strong pressure on the knob or round display
- Use the dedicated PD input when external power is needed

## Troubleshooting Notes

The original Chinese instructions include troubleshooting topics for:

- USB devices not recognized
- TF card not detected
- abnormal display behavior
- PD power not working as expected
- Wi-Fi connection issues
- incorrect time display

If you are preparing a public issue report for this repository, include:

- firmware version
- power method used
- TF card size and format
- host OS
- the exact mode where the problem occurs

## Technical Specifications Summary

The table below summarizes information gathered from the official product page and the original Chinese manual.

| Category | Details |
| --- | --- |
| Product name | HALO TOUCH USB Hub Dock with Clock V2 |
| Product type | Desktop USB hub / expansion dock with display and clock functions |
| Display | 360 x 360 round IPS screen |
| Upstream connection | 1 x USB 2.0 Type-C |
| Downstream USB | 2 x USB 2.0 Type-A, 1 x USB 2.0 Type-C |
| Card reader | TF / microSD |
| Network | 100 Mbps Ethernet |
| Extra power input | USB-C PD |
| Media support | MP3, JPG, MJPEG |
| Monitoring | Voltage / current / power per USB port |
| PC integration | AIDA64 display, Surface Dial style control |
| Wireless setup | 2.4 GHz Wi-Fi only |
| Update path | OTA update supported |

## What This Repository Is For

This repository is intended to provide:

- an English README and quick-start manual
- a structured technical summary for buyers and users
- a stable link collection for setup and review references
- a place to improve public documentation over time

## External Coverage and References

Primary sources:

- Tindie product page: [HALO TOUCH USB Hub Dock with Clock V2](https://www.tindie.com/products/johnson/halo-touch-usb-hub-dock-with-clock-v2/)
- Original Chinese manual: [pressf5.run manual page](http://pressf5.run/?p=227)
- AIDA64 setup video: [Bilibili BV1A64y1w723](https://www.bilibili.com/video/BV1A64y1w723)

Secondary coverage and discussion:

- CNX Software: [HALO TOUCH V2 – A customizable desktop USB hub with rotary encoder fitted with round touchscreen display](https://www.cnx-software.com/2026/07/03/halo-touch-v2-a-customizable-desktop-usb-hub-with-rotary-encoder-fitted-with-round-touchscreen-display/)
- Windows Forum: [Innoelement HALO TOUCH V2: Windows Rotary Hub With Touch Screen, AIDA64 & Power](https://windowsforum.com/threads/innoelement-halo-touch-v2-windows-rotary-hub-with-touch-screen-aida64-power.433788/)
- Notebookcheck coverage:
  - [Notebookcheck NL](https://www.notebookcheck.nl/Halo-Touch-V2-hub-met-geintegreerd-display-en-geavanceerde-functies.1334885.0.html)
  - [Notebookcheck FR](https://www.notebookcheck.biz/Halo-Touch-V2-hub-dote-d-un-ecran-integre-et-de-fonctionnalites-avancees.1334893.0.html)
  - [Notebookcheck ES](https://www.notebookcheck.org/Halo-Touch-V2-concentrador-con-pantalla-integrada-y-funciones-avanzadas.1334861.0.html)

## Notes on Accuracy

This README is based on publicly accessible material reviewed on **July 13, 2026**:

- the official Tindie product page
- the original Chinese instructions at `pressf5.run`
- public secondary coverage pages listed above

If the hardware, firmware, packaging, or online documentation changes later, the latest official product materials should take precedence.
