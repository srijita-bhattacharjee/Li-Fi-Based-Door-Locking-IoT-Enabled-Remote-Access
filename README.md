# Li-Fi Based Door Locking System with IoT-Enabled Remote Access

A secure smart door locking system using Li-Fi (Light Fidelity) for password transmission, combined with IoT-based remote access and user management.

## 🚀 Overview
Traditional RF/Wi-Fi-based locking systems are vulnerable to interference and hacking. This project replaces RF communication with **light-based (Li-Fi) transmission**, ensuring secure, short-range, line-of-sight authentication.

Passwords are encoded in ASCII and transmitted via LED, decoded using an LDR sensor, and verified before granting access.

## ⚙️ System Architecture

Transmitter (Arduino + LED) → Li-Fi Communication →  
Receiver (Arduino + LDR) → NodeMCU (ESP32) → Blynk Cloud  

## 🔑 Key Features
- Secure password transmission using Li-Fi (optical communication)
- ASCII-based encoding with preamble synchronization
- Real-time password verification and access control
- Remote password updates via Blynk IoT platform
- User access enable/disable functionality
- Emergency override for instant unlocking
- Low latency response (<1s)

## 🧠 System Components

### 🔹 Transmitter (Li-Fi Key)
- Arduino UNO + LED  
- Encodes password into binary and transmits via light  

### 🔹 Receiver (Door Lock Unit)
- Arduino UNO + LDR → decodes Li-Fi signal  
- Servo motor → controls locking mechanism  

### 🔹 IoT Module
- NodeMCU (ESP32) + Blynk  
- Handles:
  - Password updates  
  - User access control  
  - Emergency unlock  

## 🛠️ Tech Stack
- **Languages:** C/C++ (Arduino)
- **Microcontrollers:** Arduino UNO, ESP32
- **Communication:** Li-Fi (LED + LDR)
- **IoT Platform:** Blynk Cloud
- **Hardware:** Servo Motor, LDR, LED

## 📊 Results
- Reliable communication within 20–30 cm range  
- Accurate password decoding with preamble synchronization  
- Response time <1 second  
- Stable performance under ambient light (with calibration)  
- Seamless remote control via Blynk  

## 🔐 Security Advantages
- Line-of-sight communication prevents remote interception  
- Reduced electromagnetic interference compared to RF systems  
- Password-based authentication with user-level control  

## 📷 Demo / Setup
(Add images of circuit, setup, and working model here)

## 📁 Project Structure
