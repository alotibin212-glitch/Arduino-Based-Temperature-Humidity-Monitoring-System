# 🌡️ Arduino-Based Temperature & Humidity Monitoring System

An embedded system prototype designed to measure and display ambient environmental temperature and relative humidity in real-time. The system utilizes an Arduino Uno microcontroller, a DHT11 digital sensor, and a 16x2 character LCD screen.

---

## 🔗 Project Resources
Access the full project repository and documentation files via the link below:
[📁 Project Google Drive Folder](https://drive.google.com/drive/folders/1h4XUBORqX9rTnv4yuvm11DMNYmOQBmAT)

---

## 📊 System Architecture
The system is structured into four primary operational blocks to ensure reliable end-to-end data processing and display:

* Power Supply Block: Delivers stable 5V DC power via a Type-B USB connection.
* DHT11 Sensing Block: Samples ambient temperature and relative humidity values.
* Arduino Uno Processing Core: Decodes incoming serial streams and handles data conversion.
* LCD Output Block: A Human-Machine Interface (HMI) for clear, real-time data readability.

![System Diagram](https://github.com/user-attachments/assets/82fe52b9-0854-42b7-aa07-ca350b5447da)

---

## 🔌 Circuit Specifications
The prototype was constructed on an 830-tie-point solderless breadboard with the following interface connections:

* DHT11 Sensor: Connected via a single-wire bidirectional serial interface to Digital Pin 2, stabilized with a 10 kΩ pull-up resistor.
* 16x2 Character LCD: Operated in 4-bit mode using data lines D4–D7 mapped to Arduino Digital Pins 5, 4, 3, and 2.
* HMI Calibration: Features a 10 kΩ linear potentiometer connected to the V0 pin to adjust display contrast.

![Circuit Diagram](https://github.com/user-attachments/assets/e95bfdf0-ce53-4e8c-9762-838ff535154f)

---

## 📈 Technical Specifications

| Metric | Operational Range | Accuracy Tolerance |
| :--- | :--- | :--- |
| Ambient Temperature | 0°C to 50°C | ±2°C |
| Relative Humidity | 20% to 90% | ±5% |
| Refresh Rate | Every 2,000 ms (2s) | - |

---

## 💻 Firmware Design
Developed in C++ within the Arduino IDE, the firmware utilizes the DHT and LiquidCrystal libraries:

* `setup()` State: Initializes the LCD, prints a welcome message, and activates the sensor communication channel.
* `loop()` Routine: Executes every 2 seconds to sample sensory data, validate transmission, and update the LCD display lines.

---

## 👥 Project Team
* Eng. Fajr Aldajani - [https://github.com/Iiifajr](https://github.com/Iiifajr)
* Eng. Noura Abbad Al-Qathami - [https://github.com/alotibin212-glitch](https://github.com/alotibin212-glitch)
* Eng. Batool Falah Alguthami - [https://github.com/batoolotb90-png](https://github.com/batoolotb90-png)
* Eng. Asayel Hussain Al-Nufaiey - [GitHub Profile](#)
🔗 GitHub Profile
Affiliation: Taif University
Project Status: Completed Successfully! 🚀
