# ESP32 WiFi + Bluetooth Sniffer
![Platform](https://img.shields.io/badge/platform-ESP32-blue)
![Language](https://img.shields.io/badge/language-C++-orange)
![Type](https://img.shields.io/badge/project-IoT-green)


A lightweight RF scanner built with ESP32 that detects nearby **Wi-Fi and Bluetooth Low Energy devices** and reports their MAC addresses and signal strength (RSSI).

This project demonstrates **wireless packet sniffing, BLE scanning, and RF device detection** using only a single ESP32 board.

 Features

*  WiFi packet sniffing using ESP32 promiscuous mode
*  Bluetooth Low Energy device scanning
*  RSSI signal strength monitoring
*  Runs on a single ESP32 board (no extra hardware)
  Hardware

* ESP32 Development Board
* USB Cable
 Software

* Arduino IDE
* ESP32 Arduino Core
* BLE Library
  How It Works

The ESP32 performs two types of scanning:
1. **WiFi Sniffer**

   * Captures WiFi management frames
   * Extracts MAC address and RSSI

2. **BLE Scanner**

   * Listens for BLE advertisements
   * Detects nearby Bluetooth devices

```
Nearby Devices
     ↓
ESP32 Radio
     ↓
WiFi Sniffer + BLE Scanner
     ↓
Serial Output
```
## Example Output

```
[WiFi] 8C:AA:B5:22:9D:11 RSSI: -52
[WiFi] F4:8C:50:31:77:AB RSSI: -67

[BLE ] d3:7a:11:9c:55:21 RSSI: -70 Name: Redmi Buds
```
## Setup

1. Install **ESP32 Board Package** in Arduino IDE
2. Select your ESP32 board
3. Set partition scheme to **Huge APP (3MB No OTA)**
4. Upload the code from `src/`
## Applications

* RF monitoring
* Device presence detection
* Wireless security research
* IoT experimentation
## Disclaimer

This project is for **educational and research purposes only**. Do not use packet sniffing techniques on networks you do not own or have permission to analyze.
