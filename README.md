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

## Applications

* RF monitoring
* Device presence detection
* Wireless security research
* IoT experimentation
## Disclaimer

This project is for **educational and research purposes only**. Do not use packet sniffing techniques on networks you do not own or have permission to analyze.
