# 🌿 Smart Greenhouse App

A smart greenhouse system combining **Flutter**, **Firebase**, and **AI (VGG19)** to provide intelligent, real-time monitoring and management of plant environments. Designed for modern agriculture, it empowers users to track conditions, automate actions, and detect potential plant issues using deep learning.

---

## 📌 Project Overview

This app enables farmers and garden enthusiasts to:

- Monitor temperature, humidity, light, and soil moisture in real time.
- Automatically control irrigation, lighting, and ventilation systems.
- Receive alerts on abnormal conditions.
- Detect potential plant diseases via VGG19 image classification.
- Control everything remotely through a beautiful Flutter-based app.

---

## 🌟 Key Features

- 📲 **Cross-platform Flutter App** (Android & iOS)
- 🔥 **Firebase Integration** (Auth, Realtime Database, Storage)
- 🧠 **AI-Powered Plant Analysis** using **VGG19**
- 📡 Live sensor data from ESP32 + DHT11, Soil Moisture, LDR
- 📈 Historical data visualization (charts and logs)
- 🚨 Notifications for environmental anomalies
- 🧪 Image upload & analysis to detect leaf issues

---

## 🛠️ Technologies Used

| Category            | Tools Used                                      |
|---------------------|-------------------------------------------------|
| **Frontend**        | Flutter                                         |
| **Backend/Database**| Firebase (Auth, Realtime DB)|
| **Hardware**        | ESP32, DHT11, Soil Moisture Sensor, LDR         |
| **AI Model**        | VGG19 (TensorFlow / Python Flask API)           |
| **Communication**   | REST API / Firebase Functions                   |

---

## 🧱 System Architecture

```plaintext
[ Sensors ] → [ ESP32 ] → [ Firebase Realtime DB ]
                                ↓
                        [ Flutter Mobile App ]
                                ↓
                  [ Upload Leaf Image ] → [ Flask API + VGG19 ]
                                              ↓
                                    [ Disease Prediction ]
