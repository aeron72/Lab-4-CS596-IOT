# Lab-4-CS596-IOT  
**Lab 4: Bluetooth Step Counter with BLE and TFT Display**

Members(solo): Aeron Flores

**Video Demo Links**

Part A: https://youtube.com/shorts/sxtF72J1ahA?feature=share

Part B: https://youtube.com/shorts/W5ZLxh3JUF0?feature=share

Top Down Image (Used the same setup for both parts just left led in for Part B)
![Part Aand B](https://github.com/user-attachments/assets/6db7d229-2618-4cb6-9479-eb0e615a90dc)


## 📋 Overview
This project is part of Lab 4 for CS596 - IoT Systems. It demonstrates how to build two embedded Bluetooth Low Energy (BLE) applications using the ESP32 board:

- **Part A**: A basic BLE-controlled LED using a phone or BLE client to send "ON"/"OFF" commands.
- **Part B**: A BLE-enabled step counter that uses an LSM6DSO accelerometer to detect steps and sends the step count to a BLE client while also displaying it on a TFT screen.

---

## 📁 File Structure

| File / Folder Name       | Description                                 |
|--------------------------|---------------------------------------------|
| `Part A main`            | Main code for Part A (BLE LED control)      |
| `Part B main`            | Main code for Part B (BLE step counter)     |
| `platformio.ini Part A`  | PlatformIO configuration for Part A         |
| `platformio.ini part B`  | PlatformIO configuration for Part B         |
| `README.md`              | This file                                   |

---

## 🔧 PlatformIO Configuration

```ini
; PlatformIO Project Configuration File

[env:ttgo-lora32-v1]
platform = espressif32
board = ttgo-lora32-v1
framework = arduino
lib_deps = sparkfun/SparkFun Qwiic 6Dof - LSM6DSO@^1.0.3
monitor_speed = 115200
