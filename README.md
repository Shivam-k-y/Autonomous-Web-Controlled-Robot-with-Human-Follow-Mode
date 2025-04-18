# 🤖 Autonomous + Web Controlled Robot with Human Follow Mode

 <!-- ![Robot Banner](https://via.placeholder.com/1000x300.png?text=Autonomous+Web+Controlled+Robot) You can add your real image URL here -->

## 🚀 Project Overview

This project is a **3-in-1 Smart Robot** capable of operating in:
- 🧠 **Autonomous Obstacle Avoidance Mode**
- 🌐 **Web-Controlled Mode** via ESP8266
- 🚶 **Human Follow Mode** using IR sensors

Built using **Arduino UNO** and **ESP8266**, this robot combines real-time sensor data, smart motor logic, and wireless control into a powerful demonstration of embedded systems and IoT.

---

## 📌 Features

- **Three Operation Modes**:
  - `Mode 1:` Autonomous obstacle detection and intelligent path navigation
  - `Mode 2:` Manual control via a clean web UI (Forward, Backward, Left, Right, Stop, Speed Control)
  - `Mode 3:` Human-following using IR sensors (with distance awareness)
- **Obstacle Avoidance** with ultrasonic sensor and servo-based scanning
- **Speed Control** via slider input on web interface
- **Failsafe Timeout**: Automatically stops if no command is received for 7 seconds
- **Modular Design** using software serial, servo motor, and mode switching

---

## 🛠️ Tech Stack

| Hardware              | Software                |
|----------------------|-------------------------|
| Arduino UNO           | Arduino IDE (C/C++)     |
| ESP8266 WiFi Module   | HTML + CSS (Web UI)     |
| Ultrasonic Sensor     | ESP8266WebServer Library|
| IR Sensors (A0, A1)   | SoftwareSerial Library  |
| Servo Motor           |                         |
| Motor Driver (L298N)  |                         |
| 2WD Chassis           |                         |

---

## 🧩 Circuit Diagram

> Include a Fritzing diagram or schematic image if available.

---

## 🔌 How It Works

### ⚙️ Mode Selection
| Mode | Description                      | Command |
|------|----------------------------------|---------|
| 1    | Autonomous Mode                  | `1`     |
| 2    | Web Control Mode                 | `2`     |
| 3    | Human Follow Mode (IR + Ultra)   | `3`     |

### 🕹️ Web UI Control (Mode 2)
- Forward (`F`)
- Backward (`B`)
- Left (`L`)
- Right (`R`)
- Stop (`S`)
- Speed (`SPEEDxxx` like `SPEED200`)

### 🤖 Human Follow Logic (Mode 3)
- If **distance > 10 cm**, move forward  
- If **distance < 10 cm**, move backward  
- If **right IR sensor LOW**, turn right  
- If **left IR sensor LOW**, turn left  
- During turning, distance is **ignored**

---

---

## 👨‍💻 Team Members

- Shivam Kumar  
- Gograj Dadarwal  
- Arnav Jaiswal  
- Aadith Abhimanyu S  
- Manish Kumar  

**Special Thanks:**  
🤖 [ChatGPT](https://openai.com/chatgpt) – for continuous support during development and debugging.

---

## 💡 Future Improvements

- Add Bluetooth app control using HC-05  
- Implement camera-based object following  
- Add line-following mode using IR array  
- Introduce rechargeable power management system

---

## 📜 License

This project is open-source and free to use under the MIT License.

---



