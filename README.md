# 🔋 IoT-Based Smart Battery Charging & Monitoring System

An intelligent battery charging and monitoring system developed using **ESP32**, designed to improve charging safety through continuous monitoring of critical battery and environmental parameters. The system measures battery temperature, charging voltage, charging current, ambient temperature, and humidity in real time, while automatically controlling the charging process through relay-based protection logic.

Sensor data is displayed locally on an OLED display and simultaneously transmitted to an MQTT server for remote IoT monitoring. The system generates visual and audible alerts whenever charging conditions move outside predefined safe operating limits.

---

## 🚀 Highlights

🔋 Real-Time Battery Charging Monitoring

🌡️ Battery Temperature Monitoring using NTC Thermistor

🌤️ Ambient Temperature & Humidity Monitoring using DHT22

⚡ Charging Voltage Measurement

🔌 Charging Current Measurement

🧠 Automatic Charging Decision Logic

🔄 Relay-Based Charging Control

📟 OLED Live Status Display

☁️ MQTT-Based IoT Communication

🔔 Buzzer-Based Safety Alerts

🚦 Multi-State LED Status Indication

🛡️ Over-Temperature & Unsafe Charging Protection

---

## 🛠️ Hardware Used

* ESP32 DevKit V1
* DHT22 Temperature & Humidity Sensor
* NTC Thermistor
* SSD1306 OLED Display
* Relay Module
* Active Buzzer
* Green, Yellow & Red LEDs
* Potentiometers (Voltage & Current Simulation)
* Power Supply

---

## ⚙️ System Functions

| Module         | Function                                  |
| -------------- | ----------------------------------------- |
| DHT22          | Ambient Temperature & Humidity Monitoring |
| NTC Thermistor | Battery Temperature Monitoring            |
| OLED Display   | Live System Status Display                |
| Relay Module   | Charging Enable/Disable Control           |
| MQTT Client    | Cloud Data Transmission                   |
| LEDs           | Visual Status Indication                  |
| Buzzer         | Warning & Fault Alerts                    |
| ESP32          | Data Processing & Decision Making         |

---

## 📊 Monitoring Parameters

### Environmental Parameters

* Ambient Temperature (°C)
* Humidity (%RH)

### Battery Parameters

* Battery Temperature (°C)
* Charging Voltage (V)
* Charging Current (A)

### System Parameters

* Charging Status
* Relay Status
* Fault Condition
* Alert State

---

## 🧠 Protection Logic

The ESP32 continuously evaluates all incoming sensor data against predefined safety limits.

### ✅ Safe Charging State

* Green LED ON
* Relay ON
* Charging Enabled
* MQTT Status Updated

### ⚠️ Warning State

* Yellow LED ON
* Buzzer Activated
* Charging Paused

### 🚨 Fault State

* Red LED ON
* Continuous Alert
* Relay OFF
* Charging Disabled

This protection mechanism helps prevent unsafe charging conditions and potential battery damage.

---

## ☁️ MQTT Integration

The system publishes real-time telemetry data to an MQTT broker, enabling remote monitoring through IoT dashboards and cloud applications.

### Published Topics

* `/quillies/ambientTemperature`
* `/quillies/humidity`
* `/quillies/batteryTemperature`
* `/quillies/voltage`
* `/quillies/current`
* `/quillies/chargingStatus`

---

## 📂 Project Structure

```text
IoT-Based-Smart-Battery-Charging-Monitoring-System
│
├── sketch.ino
├── diagram.json
├── libraries.txt
├── wokwi-project.txt
├── README.md
└── images
```

## 🎯 Applications

* Electric Vehicle Battery Systems
* Smart Charging Stations
* Battery Energy Storage Systems (BESS)
* Solar Energy Storage Monitoring
* Industrial Battery Banks
* UPS & Backup Power Systems

---

## 🔮 Future Enhancements

* 📱 Blynk Mobile Dashboard
* ☁️ Cloud Data Logging
* 📈 Historical Trend Analysis
* 🔔 Push Notifications
* 🔋 State of Charge (SoC) Estimation
* ❤️ Battery Health Monitoring
* 🌐 OTA Firmware Updates
* 🤖 Predictive Fault Detection

---

## 👨‍💻 Developed By

**Ansh Dubey**

B.Tech – Electronics & Instrumentation Engineering

**ESP32 • Embedded Systems • IoT • MQTT • Battery Management • Automation**
