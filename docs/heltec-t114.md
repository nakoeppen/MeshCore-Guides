# MeshCore Device Guides - Heltec T114 <font color="red">(UNDER CONSTRUCTION)</font>
MeshCore device guides repository, with a "Keep It Simple, Stupid" flavor

[Go Back to Home](../README.md)  

![Heltec v4](https://heltec.org/wp-content/uploads/2024/08/9-1.png)

## Table of Contents  
1. [Features](#features)
2. [How-To-Use](#how-to-use)
3. [Specifications](#specifications)

## Features
- Integrated Optional Display (1.14" TFT, firmware-disableable)
- Integrated Bluetooth 5.0 Module
- Optional Battery
- Integrated Solar Input (onboard charge controller)
- Optional Enclosure
- Integrated GPS Port (8-pin GNSS connector, no soldering)
- External LoRa Antenna via IPEX connector

## How-To-Use


## Specifications
- MCU: nRF52840
- Flash: 1MB
- PSRAM: 256KB
- Radio: SX1262
- Frequency Bands: 863–928 MHz (region dependent)
- Max RF Output: ~21 dBm
- Antenna: External via IPEX
- Display: 1.14" TFT
- Power: USB-C, Battery, Solar
- Deep Sleep Current: 5mA (firmware dependent)

## General Notes
- An external LoRa antenna must be connected before transmitting to avoid damaging hardware
- TFT and GPS significantly increase power consumption and should be disabled for repeater or solar deployments
