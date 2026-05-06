#  Automated Sanitizer Dispenser System

![Platform](https://img.shields.io/badge/Platform-IoT%20System-brightgreen?logo=arduino)
![Language](https://img.shields.io/badge/Language-C%2B%2B%20%2F%20Embedded-orange?logo=cplusplus)
![IDE](https://img.shields.io/badge/IDE-Arduino%20IDE-00979D?logo=arduino)
![Sensor](https://img.shields.io/badge/Sensor-IR%20%2F%20Ultrasonic-red)
![Hardware](https://img.shields.io/badge/Hardware-Arduino%20UNO-blue)
![IoT](https://img.shields.io/badge/IoT-Touchless%20Automation-yellow)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

**Automated Sanitizer Dispenser System** is a touchless hygiene solution designed using Arduino and sensor-based automation. The system automatically dispenses sanitizer whenever a hand is detected near the sensor, reducing physical contact and improving public hygiene and safety. 🧼✨

The project is ideal for **IoT learning**, **embedded systems projects**, and **healthcare automation applications**.

---

## 🎥 Project Demo

| Demo                                | Link                          |
| ----------------------------------- | ----------------------------- |
| 🧴 Automatic Sanitizer Working Demo | Add your video/demo link here |
| ⚙️ Arduino Circuit Demonstration    | Add your demo link here       |

---

# 📌 Table of Contents

* [Features](#-features)
* [System Architecture](#-system-architecture)
* [Tech Stack](#-tech-stack)
* [Hardware Components](#-hardware-components)
* [Working Principle](#-working-principle)
* [Project Structure](#-project-structure)
* [Prerequisites](#-prerequisites)
* [Installation & Setup](#-installation--setup)
* [Circuit Connections](#-circuit-connections)
* [Arduino Compilation & Upload](#-arduino-compilation--upload)
* [Running the System](#-running-the-system)
* [Common Issues & Fixes](#-common-issues--fixes)
* [Applications](#-applications)
* [Future Enhancements](#-future-enhancements)
* [Contributing](#-contributing)
* [Author](#-author)
* [License](#-license)

---

# ✨ Features

| Feature                            | Description                                                |
| ---------------------------------- | ---------------------------------------------------------- |
| 🖐️ **Touchless Operation**        | Automatically dispenses sanitizer without physical contact |
| 📡 **Sensor-Based Detection**      | Detects hand movement using IR or ultrasonic sensor        |
| ⚡ **Fast Response System**         | Instantly activates sanitizer pump when hand is detected   |
| 🔋 **Low Power Consumption**       | Efficient embedded system suitable for continuous use      |
| 🚨 **Safe & Hygienic**             | Reduces contamination and infection spread                 |
| 🧠 **Microcontroller Automation**  | Arduino controls sensor and pump logic                     |
| 💧 **Automatic Liquid Dispensing** | Controlled sanitizer dispensing using mini pump            |
| 🏢 **Public Usage Ready**          | Suitable for schools, hospitals, malls, and offices        |

---

# 🏗️ System Architecture

```text
┌──────────────────────────────────────────────────────┐
│                  INPUT LAYER                         │
│                                                      │
│   ┌────────────────────────────┐                    │
│   │ IR / Ultrasonic Sensor     │                    │
│   │ Hand Detection Module      │                    │
│   └──────────────┬─────────────┘                    │
└──────────────────┼───────────────────────────────────┘
                   │
                   ▼
┌──────────────────────────────────────────────────────┐
│               PROCESSING LAYER                       │
│                                                      │
│              Arduino UNO / ESP32                     │
│                                                      │
│   ├── Sensor Data Processing                         │
│   ├── Distance Monitoring                            │
│   ├── Pump Control Logic                             │
│   └── Timing & Automation                            │
└──────────────────┬───────────────────────────────────┘
                   │
                   ▼
┌──────────────────────────────────────────────────────┐
│                 OUTPUT LAYER                         │
│                                                      │
│   ┌────────────────────────────┐                    │
│   │ Mini Water Pump / Motor    │                    │
│   │ Sanitizer Dispensing Unit  │                    │
│   └────────────────────────────┘                    │
└──────────────────────────────────────────────────────┘
```

---

# 🛠️ Tech Stack

| Layer                | Technology                    |
| -------------------- | ----------------------------- |
| Microcontroller      | Arduino UNO / ESP8266 / ESP32 |
| Programming Language | Embedded C++                  |
| IDE                  | Arduino IDE                   |
| Sensor               | IR Sensor / Ultrasonic Sensor |
| Output Device        | Mini Water Pump               |
| Power Supply         | USB / Battery                 |
| Automation           | Sensor-based Triggering       |

---

# 🔌 Hardware Components

| Component                     | Purpose             |
| ----------------------------- | ------------------- |
| Arduino UNO                   | Main controller     |
| IR Sensor / Ultrasonic Sensor | Hand detection      |
| Mini Water Pump               | Dispenses sanitizer |
| Relay Module / Transistor     | Controls pump       |
| Jumper Wires                  | Circuit connections |
| Breadboard                    | Prototyping         |
| Sanitizer Bottle              | Liquid storage      |
| USB Cable                     | Arduino programming |
| Power Supply                  | System power        |

---

# ⚙️ Working Principle

1. The IR or ultrasonic sensor continuously monitors nearby objects.
2. When a hand is placed near the sensor:

   * The sensor detects motion/distance.
   * Signal is sent to the Arduino.
3. Arduino processes the input signal.
4. The mini pump is activated for a few seconds.
5. Sanitizer is dispensed automatically.
6. The system returns to standby mode after dispensing.

Touchless systems significantly reduce contamination risks in public areas. ([ResearchGate][1])

---

# 📂 Project Structure

```text
Automated-Sanitizer-Dispenser/
│
├── arduino/
│   └── sanitizer_dispenser.ino      ← Arduino source code
│
├── circuit-diagram/
│   └── sanitizer_circuit.png        ← Circuit diagram
│
├── components/
│   └── hardware-list.txt            ← Required components
│
├── images/
│   └── project-preview.png          ← Project screenshots
│
├── docs/
│   └── project-report.pdf           ← Documentation
│
└── README.md
```

---

# ✅ Prerequisites

Ensure the following are installed:

| Tool               | Version | Download                                                                 |
| ------------------ | ------- | ------------------------------------------------------------------------ |
| Arduino IDE        | Latest  | [https://www.arduino.cc/en/software](https://www.arduino.cc/en/software) |
| USB Drivers        | Latest  | Arduino official website                                                 |
| Git                | Latest  | [https://git-scm.com](https://git-scm.com)                               |
| VS Code (Optional) | Latest  | [https://code.visualstudio.com](https://code.visualstudio.com)           |

---

# 🚀 Installation & Setup

## Step 1 — Clone the Repository

```bash
git clone https://github.com/Mayilraj13/Automated-Sanitizer-Dispenser-.git
cd Automated-Sanitizer-Dispenser-
```

---

## Step 2 — Open Arduino Project

1. Launch **Arduino IDE**
2. Click:

   ```
   File → Open
   ```
3. Open:

   ```
   sanitizer_dispenser.ino
   ```

---

## Step 3 — Connect Arduino

* Connect Arduino UNO via USB cable
* Wait for drivers to install

---

# 🔌 Circuit Connections

| Sensor / Module | Arduino Pin    |
| --------------- | -------------- |
| IR Sensor VCC   | 5V             |
| IR Sensor GND   | GND            |
| IR Sensor OUT   | Digital Pin 2  |
| Relay IN        | Digital Pin 8  |
| Pump VCC        | External Power |
| Pump GND        | GND            |

---

# 🔧 Arduino Compilation & Upload

## Step 1 — Select Board

Navigate:

```text
Tools → Board → Arduino UNO
```

If using ESP32:

```text
Tools → Board → ESP32 Dev Module
```

---

## Step 2 — Select COM Port

```text
Tools → Port → COMx
```

Choose the correct COM port.

---

## Step 3 — Verify the Code

Click:

```text
✔ Verify
```

Expected result:

```text
Done Compiling
```

---

## Step 4 — Upload the Code

Click:

```text
→ Upload
```

Expected result:

```text
Done Uploading
```

---

# ▶️ Running the System

1. Power the Arduino board
2. Fill sanitizer container
3. Place hand near sensor
4. Sensor detects hand movement
5. Pump activates automatically
6. Sanitizer is dispensed

---

# 🐛 Common Issues & Fixes

| Error                       | Solution                                |
| --------------------------- | --------------------------------------- |
| `Arduino not detected`      | Reconnect USB cable and install drivers |
| `COM port missing`          | Restart Arduino IDE or reconnect board  |
| `Upload failed`             | Select correct board and COM port       |
| `Pump not working`          | Check relay/transistor wiring           |
| `Sensor not detecting hand` | Adjust sensor sensitivity               |
| `Continuous dispensing`     | Modify delay timing in code             |
| `Weak sanitizer flow`       | Check pump voltage and tubing           |
| `Power issue`               | Use external power supply for pump      |

---

# 🏥 Applications

* 🏫 Schools and Colleges
* 🏥 Hospitals and Clinics
* 🏢 Offices
* 🛍️ Shopping Malls
* 🍴 Restaurants
* 🚉 Railway Stations
* ✈️ Airports
* 🏠 Smart Homes

Touchless sanitizer systems became widely adopted after COVID-19 to reduce infection spread in public spaces. ([ResearchGate][1])

---

# 🚀 Future Enhancements

* 📶 IoT monitoring using ESP8266/ESP32
* 📱 Mobile app integration
* 🔔 Low sanitizer level alert
* 📊 Usage analytics dashboard
* 🌐 Cloud data logging
* 🔋 Solar-powered operation
* 🧠 AI-based hand recognition
* 🗣️ Voice assistance integration

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch:

   ```bash
   git checkout -b feature/your-feature
   ```
3. Commit changes:

   ```bash
   git commit -m "Add your feature"
   ```
4. Push to branch:

   ```bash
   git push origin feature/your-feature
   ```
5. Open a Pull Request

---

# 👤 Author

**Mayilraj R**

* GitHub: [@Mayilraj13](https://github.com/Mayilraj13)

---

# 📄 License

This project is licensed under the **MIT License**.


