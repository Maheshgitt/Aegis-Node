# Aegis Node

## Overview

Aegis Node is an intelligent wearable safety and health monitoring system designed to provide real-time physiological and environmental monitoring for enhanced personal safety. The system integrates multiple sensors with wireless connectivity to continuously monitor vital health parameters, motion-related events, and hazardous environmental conditions.

The primary objective of Aegis Node is to create a compact, wearable device capable of acting as a personal guardian by detecting abnormal situations and providing instant alerts. By combining health monitoring, motion sensing, environmental sensing, and cloud-connected visualization, the system enables proactive safety management in both indoor and outdoor environments.

The device is built around the ESP32 microcontroller, which serves as the central processing and communication unit. Sensor data is collected, processed, displayed locally through an OLED screen, and transmitted wirelessly to a real-time web dashboard for remote monitoring.

---

## Problem Statement

Many existing wearable devices focus only on fitness tracking and lack comprehensive safety monitoring capabilities. Individuals working in hazardous environments, elderly people living independently, and people engaged in outdoor activities often require continuous monitoring of both health conditions and environmental risks.

Aegis Node addresses this challenge by integrating multiple sensing technologies into a single wearable platform capable of monitoring:

- Heart rate variations
- Body movement and orientation
- Harmful gas exposure
- Emergency conditions
- Real-time status visualization

This combination enables rapid detection of potentially dangerous situations and improves overall user safety.

---

## Key Features

### Real-Time Heart Rate Monitoring
The MAX30102 sensor continuously measures heart rate and provides real-time physiological information. The collected data helps monitor user health status and identify abnormal conditions.

### Motion and Activity Detection
The MPU6050 accelerometer and gyroscope monitor movement, orientation, and sudden changes in motion. This capability can be utilized for activity analysis and abnormal motion detection.

### Hazardous Gas Detection
The integrated gas sensor continuously measures environmental air quality and detects potentially harmful gases. When unsafe conditions are detected, alerts can be triggered immediately.

### Local OLED Display
A compact OLED display provides real-time visualization of sensor readings directly on the device, allowing users to access critical information without external devices.

### Wireless Connectivity
Using ESP32 Wi-Fi capabilities, sensor data is transmitted to a web-based dashboard for remote monitoring and visualization.

### Smart Alert System
A buzzer-based alert mechanism provides immediate audible warnings when predefined safety thresholds are exceeded.

### Live Monitoring Dashboard
A dedicated web dashboard displays sensor information in real time, enabling users or supervisors to monitor device status remotely.

---

## System Architecture

The Aegis Node architecture consists of four primary layers:

### 1. Sensing Layer
Responsible for collecting physiological and environmental data.

Sensors:
- MAX30102 Heart Rate Sensor
- MPU6050 Accelerometer and Gyroscope
- Gas Sensor

### 2. Processing Layer
The ESP32 processes incoming sensor data, performs threshold analysis, and prepares data for visualization and transmission.

### 3. Communication Layer
Wi-Fi connectivity enables wireless transmission of real-time data to the monitoring dashboard.

### 4. Visualization and Alert Layer
The OLED display, web dashboard, and buzzer provide immediate feedback and warning notifications.

---

## Hardware Components

| Component | Purpose |
|------------|------------|
| ESP32 | Main controller and Wi-Fi communication |
| MAX30102 | Heart rate monitoring |
| MPU6050 | Motion and orientation sensing |
| Gas Sensor | Air quality and gas detection |
| OLED Display | Local data visualization |
| Buzzer | Alert generation |
| Battery Supply | Portable operation |

---

## Working Principle

1. The sensors continuously collect physiological and environmental data.
2. The ESP32 processes the acquired information in real time.
3. Sensor values are displayed on the OLED screen.
4. Data is transmitted wirelessly to the monitoring dashboard.
5. Safety thresholds are continuously evaluated.
6. If abnormal conditions are detected, the buzzer activates and warning notifications can be generated.
7. The dashboard updates dynamically, allowing remote monitoring of system status.

---

## Applications

- Personal safety monitoring
- Industrial worker protection
- Smart wearable systems
- Health monitoring
- Elderly care assistance
- Outdoor activity monitoring
- Environmental hazard detection

---

## Advantages

- Real-time monitoring
- Portable and wearable design
- Wireless connectivity
- Multi-sensor integration
- Immediate alert generation
- Remote dashboard access
- Low-cost implementation
- Scalable architecture

---

## Future Enhancements

- GPS-based location tracking
- Emergency SOS messaging
- AI-powered anomaly detection
- Cloud data analytics
- Mobile application integration
- Predictive health monitoring
- Battery optimization
- Advanced wearable enclosure design

---

## Conclusion

Aegis Node demonstrates the integration of health monitoring, environmental sensing, and wireless communication into a unified wearable safety platform. The system provides continuous awareness of user conditions and surrounding environmental factors, enabling faster response to potentially dangerous situations. Its modular architecture allows future expansion into a more advanced intelligent wearable ecosystem.
