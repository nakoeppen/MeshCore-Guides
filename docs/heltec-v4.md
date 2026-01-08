# MeshCore Device Guides - Heltec v4 <font color="red">(UNDER CONSTRUCTION)</font>
MeshCore device guides repository, with a "Keep It Simple, Stupid" flavor

[Go Back to Home](../README.md)  

![Heltec v4](https://heltec.org/wp-content/uploads/2025/09/v4001.png)

## Table of Contents  
1. [Features](#features)
2. [How-To-Use](#how-to-use)
3. [Specifications](#specifications)

## Features
- Integrated Optional Display (0.96" OLED, firmware-disableable)
- Integrated WiFi/Bluetooth Modules (ESP32-S3 native)
- Optional Battery (1-cell LiPo/Li-Ion support)
- Integrated Solar Input (onboard charge controller)
- Optional Enclosure (note: V3 cases may not fit V4)
- Integrated GPS Port (8-pin GNSS connector, no soldering)
- Integrated Radio Amp (high-power SX1262 design)
- External LoRa Antenna via IPEX connector

## How-To-Use
- Connect the Heltec v4 to your computer using a USB-C cable
- Open a Chromium-based browser (Chrome, Edge, Brave)
- Navigate to the MeshCore Web Flasher
- Click **Connect Device**
- When prompted, select the Heltec v4 serial device and approve access

- If the device does not appear:
  - Hold the **BOOT / PRG** button
  - Plug in the USB cable
  - Release the button after the device connects

- Once connected, select the appropriate **Heltec v4 / ESP32-S3 (SX1262)** firmware
- Choose the desired MeshCore role:
  - **Repeater** – forwards traffic only, lowest power usage
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
- MCU: ESP32-S3
- Flash: 16MB
- PSRAM: 2MB
- Radio: SX1262
- Frequency Bands: 863–928 MHz (region dependent)
- Max RF Output: ~28 dBm
- Antenna: External via IPEX
- Display: 0.96" OLED (128x64)
- Power: USB-C, Battery, Solar
- Deep Sleep Current: 9mA (firmware dependent)

## General Notes
- Due to the integrated radio amp, TX power should be set to **22 dBm** to achieve the maximum usable RF output
- An external LoRa antenna must be connected before transmitting to avoid damaging hardware
- To boot in PROG mode without using the button, pull **GPIO0 to ground** during reset or power-up
- OLED and GPS significantly increase power consumption and should be disabled for repeater or solar deployments
