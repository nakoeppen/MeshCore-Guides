# MeshCore Device Guides
MeshCore device guides repository, with a "Keep It Simple, Stupid" flavor

### Table of Contents  
[Heltec v3](docs/heltec-v3.md)  
[Heltec v4](docs/heltec-v4.md)  
[RAK WisBlock](docs/rak-wisblock.md)  
[RAK WisMesh Tag](docs/rak-wismesh-tag.md)  
[SenseCAP Card Tracker T1000-E](docs/sensecap-card-tracker-t1000-e.md)

## High-Level Comparison
| Device | MCU | Radio | Display | Enclosure | Solar Support | Battery | WiFi | Bluetooth | GPS Support |
| ------ | --- | ----- | ------- | --------- | ------------- | ------- | ---- | --------- | ----------- |
| Heltec v3 | ESP32 | SX1262 | ✅ | Optional | ❌ | Optional | ✅ | ✅ | Yes (external, soldering) |
| Heltec v4 | ESP32-S3 | SX1262 | Optional | Optional | ✅ | Optional | ✅ | ✅ | Yes (integrated port) |
| RAK WisBlock | nRF52840 | SX1262 | ❌ | ❌ | ✅ | Optional | ❌ | ✅ | Yes |
| RAK WisMesh Tag | nRF52840 | SX1262 | ❌ | ✅ IP66 | ❌ | ✅ 1000mAh | ❌ | ✅ | Yes |
| SenseCap T1000-E | nRF52840 | SX1262 | ❌ | ✅ IP65 | ❌ | ✅ 700mAh | ❌ | ✅ | Yes |
