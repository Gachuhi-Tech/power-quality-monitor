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
