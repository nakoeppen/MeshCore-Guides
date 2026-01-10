# MeshCore Device Guides - Heltec v3 <font color="red">(UNDER CONSTRUCTION)</font>
MeshCore device guides repository, with a "Keep It Simple, Stupid" flavor

[Go Back to Home](../README.md)  

![Heltec v3](https://heltec.org/wp-content/uploads/2023/09/2.png)

## Table of Contents  
1. [Features](#features)
2. [How-To-Use](#how-to-use)
3. [Specifications](#specifications)

## Features
- Integrated Display (0.96" OLED)
- Integrated WiFi/Bluetooth Modules (ESP32)
- Optional Battery (1-cell LiPo/Li-Ion support)
- Optional Enclosure
- Integrated GPS Port (U.FL / UART, soldering required)
- External LoRa Antenna via IPEX connector
- Onboard USB-to-Serial interface

## How-To-Use
- Connect the Heltec v3 to your computer using a USB cable (Micro-USB or USB-C depending on revision)
- Open a Chromium-based browser (Chrome, Edge, Brave)
- Navigate to the MeshCore Web Flasher
- Click **Connect Device**
- When prompted, select the Heltec v3 serial device and approve access

- If the device does not appear:
  - Hold the **BOOT / PRG** button
  - Plug in the USB cable
  - Release the button after the device connects

- Once connected, select the appropriate **Heltec v3 / ESP32 (SX1262)** firmware
- Choose the desired MeshCore role:
  - **Repeater** – forwards traffic only, reduced power usage
  - **Room Server** – hosts rooms and routing state, higher uptime recommended
  - **Companion (USB or Bluetooth)** – pairs with another device for messaging or control

- Click **Flash Firmware** and wait for the process to complete
- Do not disconnect the device during flashing

- After flashing completes:
  - Click **Disconnect**
  - Power-cycle the device

- On first boot:
  - The device will initialize MeshCore storage and routing
  - For **Repeater** and **Room Server** roles, a **web-based configuration interface** is available over USB or network for setting node name, region, channel, and power options
  - OLED will display basic status information

## Specifications
- MCU: ESP32
- Flash: 4MB
- PSRAM: None
- Radio: SX1262
- Frequency Bands: 863–928 MHz (region dependent)
- Max RF Output: ~22 dBm
- Antenna: External via IPEX
- Display: 0.96" OLED (128x64)
- Power: USB, Battery
- Deep Sleep Current: ~10 µA (board), firmware dependent

## General Notes
- An external LoRa antenna must be connected before transmitting to avoid damaging hardware
- TX power should be configured according to local regulatory limits
- OLED and GPS significantly increase power consumption and should be disabled for repeater or battery-powered deployments
- GPS requires an external module and consumes power even when not actively used
- Older Heltec v3 enclosures may not accommodate all antenna or battery configurations
