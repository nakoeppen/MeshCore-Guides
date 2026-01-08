# MeshCore Device Guides
MeshCore device guides repository, with a "Keep It Simple, Stupid" flavor

### Table of Contents  
[Heltec v3](docs/heltec-v3.md)  
[Heltec v4](docs/heltec-v4.md)  
[RAK WisBlock](docs/rak-wisblock.md)  
[RAK WisMesh Tag](docs/rak-wismesh-tag.md)  
[SenseCAP Card Tracker T1000-E](docs/sensecap-card-tracker-t1000-e.md)

## High-Level Comparison
|                | MCU      | Radio    | Display                 | Enclosure               | Solar Support           | Battery                 | WiFi                    | Bluetooth               | GPS                     |
| -------------- | -------- | -------- | ----------------------- | ----------------------- | ----------------------- | ----------------------- | ----------------------- | ----------------------- | ----------------------- |
|Heltec v3       |ESP32     |SX1262    |Optional                 |Optional                 |:white_check_mark:       |Optional                 |:white_check_mark:       |:white_check_mark:       |Has Support              |
|Heltec v4       |ESP32     |SX1262    |Optional                 |Optional                 |:white_check_mark:       |Optional                 |:white_check_mark:       |:white_check_mark:       |Has Support              |
|RAK WisBlock    |nRF52840  |SX1262    |:x:                      |:x:                      |:white_check_mark:       |Optional                 |:white_check_mark:       |:white_check_mark:       |Has Support              |
|RAK WisMesh Tag |nRF52840  |SX1262    |:x:                      |:white_check_mark:IP66   |:x:                      |:white_check_mark:1000mAh|:x:                      |:white_check_mark:       |:white_check_mark:       |
|SenseCap T1000-E|nRF52840  |SX1262    |:x:                      |:white_check_mark:IP65   |:x:                      |:white_check_mark:700mAh |:white_check_mark:       |:white_check_mark:       |:white_check_mark:       |
