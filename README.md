# Arduino-PWM-MOSFET-Fan-Speed-Controller

[![Arduino](https://img.shields.io/badge/Arduino-Prototyping-00979D?style=for-the-badge&logo=arduino)](https://www.arduino.cc/)
[![Category](https://img.shields.io/badge/Category-Power_Electronics_&_Drivers-00e5ff?style=for-the-badge)](#)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](#)
[![Author](https://img.shields.io/badge/Author-Pranjal_Das-orange?style=for-the-badge)](https://github.com/iPranjalDas)

💨 High-power 15A 400W dual MOSFET PWM speed regulator with infrared NEC remote control decoding.

---

## 🖥️ System Architecture & Visual Wiring Layout

### 🔌 Graphical Schematic & Pinout Diagrams

![How To Make a DC Fan Speed Controller using Arduino and IR Remote](How%20To%20Make%20a%20DC%20Fan%20Speed%20Controller%20using%20Arduino%20and%20IR%20Remote.png)

![15A 400W MOSFET Trigger Switch Drive Module](15A%20400W%20MOSFET%20Trigger%20Switch%20Drive%20Module.png)



```
┌── HIGH-CURRENT MOSFET PWM SPEED REGULATION ─────────────────────────────┐
│                                                                         │
│   [IR Receiver (TSOP1738)]              [15A 400W MOSFET Module]        │
│   OUT ──> Digital Pin 11                PWM Trigger ──> Digital Pin 9   │
│   VCC ──> 5V                            GND         ──> Ground          │
│   GND ──> Ground                                                        │
│                                         [High-Power DC Load]            │
│   [Infrared Remote]                     VIN+ ──> 12V-36V Battery/PSU    │
│   • Power: Toggle On/Off                MOTOR+ ──> High-Current Fan     │
│   • Speed +/-: 0-255 PWM Duty Cycle     MOTOR- ──> Low-Side MOSFET Drain│
│   • Presets: 25%, 50%, 75%, 100%                                        │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## 🛠️ Hardware Requirements & Components

- **Microcontroller / Core:** Arduino Uno / ESP32 / NodeMCU (Refer to `.ino` sketch)
- **Power Supply:** 5V / 12V external regulated battery pack
- **Sensors & Actuators:** Detailed in circuit diagram and sketch pinout headers

---

## 🚀 Installation & Upload

1. Clone this repository:
   ```bash
   git clone https://github.com/iPranjalDas/Arduino-PWM-MOSFET-Fan-Speed-Controller.git
   ```
2. Open the primary `.ino` sketch in the [Arduino IDE](https://www.arduino.cc/en/software).
3. Install required libraries via the Arduino Library Manager.
4. If this sketch uses Wi-Fi, update `YOUR_WIFI_SSID` and `YOUR_WIFI_PASSWORD` with your local network settings.
5. Select your target board and COM port, then click **Upload**.

---

## 🔒 Security & Privacy Notice
All source sketches have been thoroughly sanitized. Generic placeholder strings are used for network credentials and API tokens.

---

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.  
Copyright (c) 2026 Pranjal Das. All Rights Reserved.

---

## 👤 Author & Architecture
**Pranjal Das**  
- **GitHub:** [@iPranjalDas](https://github.com/iPranjalDas)
- **Projects:** [https://iPranjalDas.github.io/Projects/](https://iPranjalDas.github.io/Projects/)
