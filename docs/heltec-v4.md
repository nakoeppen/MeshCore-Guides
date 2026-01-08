# MeshCore Device Guides - Heltec v4 <font color="red">(UNDER CONSTRUCTION)</font>
MeshCore device guides repository, with a "Keep It Simple, Stupid" flavor

[Go Back to Home](../README.md)  

![Heltec v4](https://heltec.org/wp-content/uploads/2025/09/v4001.png)

## Table of Contents  
1. [Features](#features)
2. [How-To-Use](#how-to-use)
3. [Specifications](#specifications)

## Features
- Integrated Optional Display
- Integrated WiFi/Bluetooth Modules
- Optional Battery
- Integrated Solar Input
- Optional Enclosure
- Integrated GPS Port
- Integrated Radio Amp
- Dedicated PROG and RESET buttons

## How-To-Use


## Specifications
- MCU: ESP32-S3R2
- Radio: SX1262
- Interfaces: USB Type C
- Memory: 16MB Flash / 2MB PSRAM

## General Notes
- Due to the integrated radio amp, TX power should be set to 22 to achieve the maximum power supported by the board
- To boot in PROG mode without use the button, put GPIO0 to ground
