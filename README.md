# ⚡ Power Quality Monitor

An ESP32-based IoT Power Quality Monitoring and Protection System designed to monitor electrical parameters in real time and automatically protect connected loads from abnormal power conditions.

The system continuously measures voltage and current, calculates electrical parameters, displays live data through a built-in web dashboard, and disconnects the load whenever unsafe operating conditions are detected.

This project demonstrates the integration of embedded systems, electronics, IoT communication, and web technologies to create a reliable smart energy monitoring solution.

## 📌 Problem Statement

Power quality disturbances such as overvoltage, undervoltage, and overcurrent can damage electrical equipment, reduce system reliability, and increase maintenance costs.

Many low-cost monitoring solutions only display electrical measurements without providing automatic protection or remote monitoring capabilities.

This project addresses these challenges by developing an ESP32-based IoT Power Quality Monitor capable of continuously monitoring electrical parameters, detecting abnormal operating conditions, and automatically disconnecting the load to improve safety and equipment protection.

## 🎯 Project Objectives

The main objective of this project is to design and implement an IoT-based power quality monitoring and protection system using the ESP32 microcontroller.

### Specific Objectives

- Monitor AC voltage in real time.
- Measure load current continuously.
- Calculate electrical parameters such as power and energy.
- Detect overvoltage, undervoltage, and overcurrent conditions.
- Automatically disconnect the load during fault conditions.
- Display real-time measurements through a web dashboard.
- Provide a scalable platform for future cloud integration and data logging.

## ✨ Key Features

### Electrical Monitoring
- Real-time AC voltage measurement
- Real-time load current measurement
- Active power calculation
- Energy consumption monitoring
- Power factor estimation

### Protection System
- Overvoltage detection
- Undervoltage detection
- Overcurrent detection
- Automatic relay-based load isolation
- Safe power restoration

### IoT Capabilities
- Built-in ESP32 web server
- Live monitoring dashboard
- Wi-Fi connectivity
- Real-time parameter updates

### User Interface
- Easy-to-read web dashboard
- Live system status indicators
- Fault notifications
- Protection event display

### Expandability
- Cloud integration ready
- Data logging ready
- Mobile application ready
- MQTT support (planned)

## 📷 System Preview

> Screenshots, hardware images, circuit diagrams, and the web dashboard will be added as development progresses.

## 🏗️ System Architecture

The Power Quality Monitor is built around the ESP32 microcontroller, which continuously acquires electrical measurements, processes the data, evaluates protection conditions, and serves live information through an integrated web dashboard.

The system consists of four major subsystems:

1. **Measurement System**
   - Voltage sensing using the ZMPT101B sensor
   - Current sensing using a current transformer (CT)

2. **Processing Unit**
   - ESP32 microcontroller
   - Signal processing
   - Power quality calculations
   - Protection logic

3. **Protection System**
   - Relay control
   - Overvoltage protection
   - Undervoltage protection
   - Overcurrent protection

4. **Monitoring Interface**
   - Built-in HTTP web server
   - Real-time dashboard
   - Wi-Fi connectivity

## 🔄 System Data Flow

```text
AC Supply
     │
     ▼
Voltage Sensor (ZMPT101B)
Current Transformer (CT)
     │
     ▼
ESP32 ADC
     │
     ▼
Signal Processing
     │
     ▼
Power Quality Calculations
     │
     ├──────────────► Web Dashboard
     │
     ▼
Protection Logic
     │
     ▼
Relay Driver
     │
     ▼
Protected Load
```

## 🔌 Hardware Components

| Component | Purpose |
|-----------|---------|
| ESP32 DevKit V1 | Main controller |
| ZMPT101B Voltage Sensor | AC voltage measurement |
| Current Transformer (CT) | AC current measurement |
| Relay Module | Load protection |
| Wi-Fi Network | Remote monitoring |
| AC Load | System under monitoring |

## 💻 Software Architecture

The firmware follows a modular architecture to improve readability, maintainability, and future scalability.

### Software Modules

| Module | Responsibility |
|---------|----------------|
| Sensor Manager | Reads voltage and current sensors |
| Calculation Engine | Computes RMS voltage, current, power, energy, and power factor |
| Protection Manager | Detects abnormal conditions and controls the relay |
| Web Server | Hosts the real-time monitoring dashboard |
| Display Manager | Updates local display (if installed) |
| Configuration Manager | Stores Wi-Fi and system settings |
| Main Controller | Coordinates all system operations |

## 🛠️ Development Environment

| Tool | Purpose |
|------|---------|
| Arduino IDE | Firmware development |
| ESP32 Arduino Core | ESP32 programming framework |
| Git | Version control |
| GitHub | Source code management |
| Proteus | Circuit simulation |
| Web Browser | Dashboard monitoring |

## 📁 Project Structure

```text
power-quality-monitor/
│
├── firmware/        ESP32 source code
├── hardware/        Schematics, PCB and Proteus files
├── docs/            Technical documentation
├── images/          Screenshots and photographs
├── web/             Dashboard resources
├── tests/           Testing procedures and results
└── README.md        Project documentation
```

## 🚀 Getting Started

### Requirements

- ESP32 Development Board
- Arduino IDE
- ESP32 Arduino Core
- ZMPT101B Voltage Sensor
- Current Transformer (CT)
- Relay Module

### Installation

1. Clone this repository.
2. Open the firmware project in Arduino IDE.
3. Install the required ESP32 board package.
4. Configure Wi-Fi credentials.
5. Upload the firmware to the ESP32.
6. Access the web dashboard using the ESP32 IP address.


## 🧪 Testing & Validation

The system will be validated through functional testing, electrical measurements, and protection response verification.

### Test Cases

| Test | Expected Result |
|------|-----------------|
| Normal Operation | Relay remains ON and live measurements are displayed |
| Overvoltage | Relay disconnects the load |
| Undervoltage | Relay disconnects the load |
| Overcurrent | Relay disconnects the load |
| Wi-Fi Connection | Web dashboard becomes accessible |
| Dashboard Refresh | Live values update correctly |

Future versions will include measured response times, accuracy analysis, and calibration results.


## 🚀 Future Improvements

Planned enhancements include:

- MQTT cloud integration
- Historical data logging
- Mobile application
- OTA firmware updates
- SD card storage
- Three-phase power monitoring
- Harmonic analysis
- Frequency monitoring
- Remote firmware management
- User authentication for the web dashboard

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## 👨‍💻 Author

**Peter Ruthi**

Bachelor of Science in Electronics & Computer Technology  
Mount Kenya University

- GitHub: https://github.com/Gachuhi-Tech
-  LinkedIn: www.linkedin.com/in/peter-ruthi-816972245

## 🙏 Acknowledgements

Special thanks to the open-source community and the developers of the ESP32 platform, Arduino ecosystem, and supporting libraries that made this project possible.




