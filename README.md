# 🩺 Elder Fall Detection System

A smart IoT-based wearable system designed to monitor elderly individuals, detect falls in real time, and provide live location tracking. The system uses motion data from an accelerometer and automatically updates a cloud database, enabling caregivers to monitor the user's status through a mobile application.

## 🚀 Features

* 📡 Real-time monitoring using ESP32
* 🏃 Activity detection (SAFE / ACTIVE / FALL)
* 🚨 Instant fall detection and alert generation
* 📍 Live GPS location tracking
* ☁️ Firebase Realtime Database integration
* 📱 Flutter-based mobile application
* 📊 Event logging and sensor data visualization
* 🔄 Continuous cloud synchronization

## 🛠️ Tech Stack

### Hardware

* ESP32
* MPU6050 Accelerometer & Gyroscope
* GPS Module

### Software

* Flutter
* Firebase Realtime Database
* Arduino IDE

## 🏗️ System Architecture

```text
MPU6050 + GPS
       │
       ▼
     ESP32
       │
       ▼
Firebase Realtime Database
       │
       ▼
 Flutter Mobile App
       │
       ▼
 Caregiver / User Monitoring
```

## ⚙️ Working Principle

1. The MPU6050 continuously measures acceleration and motion data.
2. ESP32 processes sensor readings to determine the user's state:

   * ✅ SAFE
   * 🚶 ACTIVE
   * 🚨 FALL
3. GPS coordinates are collected in real time.
4. Sensor status and location data are uploaded to Firebase.
5. The Flutter application retrieves and displays:

   * Current status
   * Live location
   * Historical event logs
6. When a fall is detected, an alert is immediately generated.

## 📱 Application Screenshots

### Dashboard

<img width="1080" height="2392" alt="Dashboard" src="https://github.com/user-attachments/assets/19088286-af6b-40fd-885e-b6107bf9e92e" />

### Event History

<img width="1080" height="2392" alt="History" src="https://github.com/user-attachments/assets/04e6d456-e0dc-44ee-b7b1-a0a08c014861" />

### Live Monitoring

<img width="1080" height="2392" alt="Monitoring" src="https://github.com/user-attachments/assets/a518cd7e-dcbd-4900-b6fe-f3b18b6139ad" />

### Hardware Prototype

<img width="954" height="576" alt="Prototype" src="https://github.com/user-attachments/assets/2136a105-0b87-4bd2-9fa3-bcad024f7d8e" />

## 📊 Status Definitions

| Status | Description                              |
| ------ | ---------------------------------------- |
| SAFE   | User is stationary and normal            |
| ACTIVE | User is moving normally                  |
| FALL   | Sudden abnormal motion indicating a fall |

## 🎯 Project Objectives

* Improve elderly safety and independence
* Provide real-time emergency awareness
* Enable remote monitoring by caregivers
* Deliver a low-cost and scalable healthcare solution

## 🔮 Future Enhancements

* SMS and phone-call alerts
* Emergency contact integration
* Geofencing support
* Heart rate and SpO₂ monitoring
* Machine Learning based fall classification
* Battery optimization for long-term deployment

## 👨‍💻 Team

Developed as part of **Hack30 2026**.

A practical IoT healthcare solution focused on enhancing elderly safety through real-time monitoring, fall detection, and location tracking.
