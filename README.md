
# Gesture Operated Vehicle System (GOVS) 🚗🖐️

**GOVS** (Gesture Operated Vehicle System), also known as **HandiCar**, is a real-time, gesture-controlled robotic vehicle designed for intuitive hands-free navigation. It uses motion sensors and wireless communication to allow users—especially individuals with physical impairments—to control a car with hand gestures.

## 🧠 Motivation

Traditional control methods like joysticks or smartphone apps are not universally accessible. GOVS aims to overcome these limitations by offering a **gesture-based**, **low-cost**, and **real-time** control system that is:
- Easy to use
- Responsive
- Assistive in nature
- Expandable to smart mobility and automation applications

---

## 🚀 Features

- **MPU6050-based gesture control**
- **Bidirectional RF communication** using nRF24L01+
- **Obstacle detection and rerouting** using HC-SR04 ultrasonic sensor + servo scanning
- **Low power mode** for idle states
- **OLED status display** on controller side
- **Emergency stop system**
- **Multidirectional Mecanum wheel chassis**
- **Visual feedback using RGB LEDs**
- **Expandable to voice control and mobile app integration**

---

## 📦 System Architecture

```plaintext
[MPU6050 Sensor] 
     ↓
[Arduino Controller] 
     ↓
[nRF24L01 Transmitter] 
     ↔
[nRF24L01 Receiver] 
     ↓
[Arduino Car] → [Motors, LED Indicators, Sensors]
```

---

## 🧩 Subsystems

- **Gesture Input Subsystem:** Maps pitch and roll angles to x/y axis control values.
- **Communication Subsystem:** RF-based data transfer with ACK and feedback.
- **Motion Subsystem:** Mecanum wheels allow forward, backward, rotation, and lateral motion.
- **Obstacle Detection:** Servo-mounted ultrasonic sensor with dual-phase avoidance + emergency stop.
- **User Feedback:** OLED on controller + RGB LEDs on vehicle.
- **Power Management:** Low power and emergency modes.

---

## 📂 Repository Structure

```
GOVS/
├── codes/
│   ├── transmitter.ino
│   └── receiver.ino
├── docs/
│   ├── ECE49200 - Final Report.pdf
│   └── Poster.pdf
├── images/
│   └── system_diagram.png
└── README.md
```

---

## ⚙️ Technologies Used

- **Microcontrollers:** Arduino Uno & Nano
- **Wireless Module:** NRF24L01+
- **Motion Sensor:** MPU6050
- **Ultrasonic Sensor:** HC-SR04
- **Motor Driver:** L298N
- **Display:** SSD1306 OLED
- **Programming Language:** C++
- **IDE:** Arduino IDE


---

## 📈 Future Improvements

- AI-based gesture classification using ML
- Voice command fallback mode
- Mobile app integration (via BLE)
- Enhanced obstacle mapping using multiple sensors
- Cloud-based data logging and analytics

---

## 👨‍💻 Authors

This project was developed by the **HandiCar Team** as part of ECE49200 at Purdue University:

- Amit Vardhan Suryadevara
- Biak Par
- Divya Patel
- Maha Ali
- Martine Cardichon
- Yamini Sri Krubha

Project Supervisor: **Prof. Greg Sturm**

---

## 📄 License

This project is for educational and research purposes. For inquiries about reuse or contributions, please contact the project authors.

---

## 🌐 Standards Compliance

This system adheres to:
- **ISO/IEC 30113-1:2025** (Gesture-based interface)
- **ISO/IEC 25010** (System & Software Quality Model)

---

## 📷 Screenshots

![System Architecture](images/system_diagram.png)
*(Add your own diagrams or screenshots here)*

---

## 🧠 ABET Learning Outcomes

This capstone project fulfills multiple ABET outcomes including:
- Problem solving
- Engineering design
- Team collaboration
- Communication
- Ethics & constraints awareness
