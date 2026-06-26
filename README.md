# 🚨 SENTINEL

## Sewer Environmental Network for Threat Intelligence and Environmental Learning

## 📖 Project Overview

**SENTINEL (Sewer Environmental Network for Threat Intelligence and Environmental Learning)** is an intelligent IoT-based sewer monitoring system designed to improve worker safety and environmental surveillance through real-time sensing and AI-powered analytics.

The system continuously monitors hazardous gases, temperature, humidity, and air quality while performing AI-based pest detection using an ESP32-S3 Camera Module. Environmental data is transmitted via MQTT to Firebase Cloud and visualized through an interactive web dashboard for centralized monitoring and rapid decision-making.

## 🎯 Objectives

* Monitor hazardous sewer gases in real time.
* Measure environmental parameters continuously.
* Detect pests using Deep Learning.
* Provide instant alerts for dangerous conditions.
* Store sensor data securely in the cloud.
* Enable centralized monitoring through a web dashboard.
* Improve worker safety and preventive maintenance.

# ✨ Key Features

* 🌍 Real-time Environmental Monitoring
* ☣ Hazardous Gas Detection
* 🌡 Temperature & Humidity Monitoring
* 🤖 AI-powered Pest Detection
* 📡 MQTT-based Data Communication
* ☁ Firebase Cloud Integration
* 📊 Interactive Web Dashboard
* 📈 Historical Data Visualization
* 🚨 Intelligent Alert System
* 📍 Scalable Multi-node Architecture

# 🏗 System Architecture

```
                                     ┌──────────────────────────────┐
                                    │      Sewer Environment       │
                                    └──────────────┬───────────────┘
                                                   │
                  ┌────────────────────────────────┼────────────────────────────────┐
                  │                                │                                │
          ┌───────▼────────┐              ┌────────▼────────┐              ┌────────▼────────┐
          │  MQ-7 Sensor   │              │ MQ-135 Sensor   │              │ DHT11 Sensor    │
          │ Carbon Monoxide│              │ Air Quality &   │              │ Temperature &   │
          │ Detection       │              │ Toxic Gases     │              │ Humidity        │
          └───────┬────────┘              └────────┬────────┘              └────────┬────────┘
                  └────────────────────────────────┼────────────────────────────────┘
                                                   │
                                           ┌───────▼────────┐
                                           │     ESP32      │
                                           │ Edge Controller│
                                           │ Data Processing│
                                           └───────┬────────┘
                                                   │
                              Threshold-Based Hazard Detection
                                                   │
                 ┌─────────────────────────────────┼─────────────────────────────────┐
                 │                                 │                                 │
        ┌────────▼────────┐              ┌────────▼────────┐              ┌────────▼────────┐
        │ ESP32-S3 Camera │              │ MQTT Protocol   │              │ Wi-Fi Network   │
        │ Image Capture   │              │ Data Transfer   │              │ Communication   │
        └────────┬────────┘              └────────┬────────┘              └─────────────────┘
                 │                               │
        ┌────────▼────────┐                      │
        │ MobileNetV3 +   │                      │
        │ CBAM AI Model   │                      │
        │ Pest Detection  │                      │
        └────────┬────────┘                      │
                 └──────────────┬────────────────┘
                                │
                      ┌─────────▼──────────┐
                      │ Firebase Realtime  │
                      │      Database      │
                      └─────────┬──────────┘
                                │
          ┌─────────────────────┼─────────────────────┐
          │                     │                     │
 ┌────────▼─────────┐  ┌────────▼─────────┐  ┌────────▼─────────┐
 │ Live Dashboard   │  │ Historical Data │  │ Hazard Alerts    │
 │ Environmental UI │  │ Trends & Charts │  │ Safe / Warning / │
 │                  │  │                 │  │ Hazardous Status │
 └──────────────────┘  └─────────────────┘  └──────────────────┘
```

## 🚀 Architecture Workflow
```
🌍 Sewer Environment
        │
        ▼
📡 IoT Sensors (MQ-7 • MQ-135 • DHT11)
        │
        ▼
🧠 ESP32 Edge Processing
        │
        ├── Threshold-Based Gas Analysis
        ├── Environmental Monitoring
        └── ESP32-S3 Camera
                │
                ▼
         🤖 MobileNetV3 + CBAM
          AI Pest Classification
                │
                ▼
        📶 MQTT over Wi-Fi
                │
                ▼
      ☁ Firebase Realtime Database
                │
        ┌───────┼────────┐
        ▼       ▼        ▼
📊 Live Dashboard  📈 Analytics  🚨 Smart Alerts

```
# 🛠 Hardware Components

| Component       | Purpose                           |
| --------------- | --------------------------------- |
| ESP32           | Main IoT Controller               |
| ESP32-S3 Camera | AI-based Pest Detection           |
| MQ-7            | Carbon Monoxide Detection         |
| MQ-135          | Air Quality & Toxic Gas Detection |
| DHT11           | Temperature & Humidity            |
| Wi-Fi Module    | Wireless Communication            |

# 💻 Software & Technologies

* Arduino IDE
* Python
* HTML
* CSS
* JavaScript
* Firebase Realtime Database
* Firebase Authentication
* MQTT Protocol
* MobileNetV3
* CBAM
* Google Colab
* Git & GitHub

# 🤖 AI Model

### Model Used

* MobileNetV3-Large
* CBAM (Convolutional Block Attention Module)

### Dataset

The pest classification model was trained using a custom dataset created by combining multiple publicly available datasets.

### Classes

* Cockroach
* Mosquito
* Larva
* Drain Fly
* Beetle
* Armyworm
* Sawfly

# 📊 Dashboard Features

The web dashboard provides:

* Live Environmental Monitoring
* Hazard Status
* Real-time Gas Values
* Temperature Trends
* Humidity Trends
* Air Quality Monitoring
* Pest Detection Results
* Historical Data
* Responsive UI
* Firebase Integration

# ☁ Cloud Database

Firebase Realtime Database stores:

* Temperature
* Humidity
* MQ7 Values
* MQ135 Values
* Gas Status
* Air Quality
* Hazard Level
* Pest Detection Results
* Timestamp
* Node Information

# 📡 Data Flow

```
Sensors
   │
   ▼
ESP32
   │
Threshold Algorithm
   │
MQTT
   │
Firebase
   │
Web Dashboard
   │
User
```

# 📈 Expected Outcomes

* Early Hazard Detection
* Continuous Environmental Monitoring
* AI-assisted Pest Identification
* Remote Monitoring
* Faster Decision Making
* Reduced Manual Inspection
* Improved Worker Safety

# 🚀 Future Enhancements

* Multi-node Deployment
* Mobile Application
* SMS & Email Alerts
* Predictive Analytics
* Edge AI Inference
* Live Camera Streaming
* GIS-based Monitoring
* Automated Report Generation

# 🎓 Academic Information

**Project Title**

SENTINEL: Sewer Environmental Network for Threat Intelligence and Environmental Learning

**Domain**

Embedded Systems • Internet of Things (IoT) • Artificial Intelligence • Environmental Monitoring

# 👨‍💻 Team

* Karthick Raja P
* Karunya R
* Mohammed Raeef I

**Supervisor**

Dr. G. Ayappan
Assistant Professor
Department of Electronics and Communication Engineering

# 📚 References

* Smart Drainage Monitoring System using IoT
* MobileNetV3 for Efficient CNN Models
* CBAM: Convolutional Block Attention Module
* MQTT Protocol Documentation
* Firebase Documentation

# 📜 License

This project is developed for academic and research purposes under the Department of Electronics and Communication Engineering.

## ⭐ If you found this project useful, consider giving it a star on GitHub!

This version is cleaner, more modern, and follows the style commonly seen in professional GitHub repositories, making it suitable for portfolios and recruiter review.
