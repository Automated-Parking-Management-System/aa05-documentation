# Automated Parking Management System
**Computer/Electrical Engineering Capstone Design Project**

Toronto Metropolitan University, W2024

By:
- Taskin Abdur-Rahman
- Zohraan Badar
- Kisoban Rajendran
- Yadu Krishnan Madhu

---

## Acknowledgement
We would like to express our sincere gratitude to all those who contributed to the successful completion of this engineering design report. Special thanks to:
- **Dr. Alagan Anpalagan**, The Faculty Lab Coordinator (FLC), for his guidance and assistance.
- **ECB Department**, for facilitating the capstone design project experience.

We also appreciate the support of our peers and the resources provided by the **Faculty of Engineering and Architectural Science**.

---

## Certification of Authorship
“I hereby certify that I/we are the author(s) of this document, and any assistance I/we received in its preparation is fully acknowledged. All sources are properly cited.”

- **Taskin Abdur-Rahman**
- **Zohraan Badar**
- **Kisoban Rajendran**
- **Yadu Krishnan Madhu**

---

## Table of Contents
1. [Acknowledgement](#acknowledgement)
2. [Certification of Authorship](#certification-of-authorship)
3. [Abstract](#abstract)
4. [Introduction & Background](#introduction--background)
5. [Objectives](#objectives)
6. [Theory and Design](#theory-and-design)
    - [Parking Lot Authentication](#parking-lot-authentication)
    - [QR-Code](#quick-response-qr-code)
    - [Parking Presence Detection](#parking-presence-detection)
    - [Firebase](#firebase-baas)
7. [Material/Component list](#materialcomponent-list)
8. [Measurement and Testing Procedures](#measurement-and-testing-procedures)
9. [Analysis of Performance](#analysis-of-performance)
10. [Conclusion](#conclusion)
11. [References](#references)

---

## Abstract
Parking lots, especially in areas like airports, malls, and downtown, face congestion due to unorganized traffic flow. This report proposes an **Automated Parking Management System (APMS)** using IoT technology and sensors for touch-free parking automation, authentication, and real-time monitoring.

The system includes:
- QR code authentication
- Automatic license plate recognition
- Predictive analytics for spot availability

This design improves cost-efficiency and security. Alternative methods like **RFID technology** are explored to enhance performance.

---

## Introduction & Background
Parking lots are often crowded, especially in high-traffic areas such as airports or malls. This project aims to create a fully automated parking management system that is **touch-free, time-efficient**, and **user-friendly**.

The parking system will:
- Automate parking spot monitoring using sensors
- Provide QR code-based entry and exit authentication
- Enable users to book parking spots through a **web application**

---

## Objectives
Key objectives for the **Automated Parking Management System (APMS)** include:
- Automating parking lot processes using **IoT** and **real-time data**.
- Providing a **GUI** for booking and predicting spot availability.
- Supporting multiple types of parking spots (e.g., regular, premium, disabled).

---

## Theory and Design

### Parking Lot Authentication
Users authenticate using **QR Codes** at the parking lot gate. The **ESP32-CAM** captures the QR code, uploads it to a cloud database, and a server opens the gate if valid.

### Quick Response (QR)-Code
QR codes store data in a two-dimensional grid, scanned by smartphones. This allows for touch-free entry into the parking lot.

### Parking Presence Detection
A **weight sensor** detects when a car occupies a spot, updating the system and triggering lights to indicate availability.

### Firebase (BaaS)
Firebase is used to manage real-time databases, authentication, and cloud storage for the parking lot system.

---

## Material/Component List
| Description | Quantity | Cost | Total |
|-------------|----------|------|-------|
| ESP32-CAM   | 2        | $34.99| $39.54|
| Breadboard  | 1        | $16.99| $19.20|
| Load Cell   | 6        | $3.32 | $22.51|

---

## Measurement and Testing Procedures
**Weight Sensor Calibration** is performed using known weights and measuring the sensor’s response to establish a baseline for car detection.

---

## Analysis of Performance
QR code reading performance was measured in three categories:
1. **Digitally generated images**: 100% success rate.
2. **Real-time images**: Limited success with ESP32-CAM.
3. **Use case performance**: High failure rate due to poor image quality.

---

## Conclusion
The **Automated Parking Management System (APMS)** offers a reliable, user-friendly solution to parking lot congestion. Future improvements may include exploring **RFID technology** and refining QR code detection for better performance.

---

## References
- Google Firebase: [https://firebase.google.com/](https://firebase.google.com/)
- Keras: [https://keras.io/](https://keras.io/)
