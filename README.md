# 🚗 Advanced Cruise Control System

An intelligent driver-assistance prototype built using embedded systems and Simulink, designed to automate vehicle speed control based on real-time obstacle detection. Developed using Raspberry Pi, ultrasonic sensors, a camera module, and DC motor simulation.

---

## 🧠 Abstract

Long-distance driving often results in fatigue and slower human reaction, increasing the chance of accidents. This project presents a real-time **Advanced Cruise Control (ACC)** system using a Raspberry Pi, camera module, and ultrasonic sensor. It dynamically adjusts vehicle speed based on object detection and distance sensing. A DC motor simulates vehicle motion, and MATLAB/Simulink models validate the control logic. The system demonstrates efficient integration of real-time sensing and actuation for smart, safer mobility solutions.

---

## 🌟 Features

- Real-time distance measurement using ultrasonic sensor.
- Basic object detection with camera.
- Dynamic motor speed adjustment (acceleration, deceleration, stop).
- Simulink-based simulation of ego and lead vehicle dynamics.
- Braking system simulation using ABS-like slip ratio control.

---

## 🛠️ System Overview

**Control Unit:** Raspberry Pi  
**Sensors:** Ultrasonic Sensor (HC-SR04), Raspberry Pi Camera Module  
**Actuator:** DC Motor  
**Simulation Platform:** MATLAB/Simulink  
**Control Logic:** PWM-based speed control with distance feedback


---

## 🔩 Hardware Components

| Component            | Quantity | Description                       |
|----------------------|----------|-----------------------------------|
| Raspberry Pi         | 1        | Central processing unit           |
| Ultrasonic Sensor    | 1        | Obstacle detection (2cm–400cm)    |
| Camera Module        | 1        | Object presence detection         |
| DC Motor             | 1        | Simulates vehicle speed           |
| Motor Driver (L298N) | 1        | Controls motor via PWM            |
| Jumper Wires         | 30       | Hardware interfacing              |
| Breadboard           | 1        | Prototyping base                  |

---

## 🧪 Simulation Model

Simulation was implemented using MATLAB/Simulink to:

- Test control logic before hardware implementation
- Simulate lead and ego car dynamics
- Evaluate acceleration, speed, and safe distance in real-time

Also includes ABS-based braking simulation to prevent wheel lock.
![sim](https://github.com/user-attachments/assets/bae946a8-2885-4e28-a336-a870f59f78b1)
![hardware implementation](https://github.com/user-attachments/assets/14245ad0-5948-4031-bbb2-5f0e01175f28)
![connection](https://github.com/user-attachments/assets/929c2852-9b0e-4a12-8ae6-94df603001fc)



---

## ✅ Results

- Successfully maintained a safe distance using sensor data.
- Smooth deceleration and re-acceleration when obstacles were detected and cleared.
- Braking simulation brought vehicle to stop within 15s under safe slip conditions.
- Hardware implementation confirmed PWM adjustments based on ultrasonic feedback.
<img width="721" height="604" alt="acc simulation results" src="https://github.com/user-attachments/assets/b812aebd-6986-4971-986b-b3f471bfbdcd" />
<img width="654" height="567" alt="abs results" src="https://github.com/user-attachments/assets/e283c199-b8ea-4c5a-87b4-d32faa4feef2" />


---

## 🚀 Applications

- Highway driving assistance  
- Stop-and-go traffic navigation  
- Enhanced driver comfort and safety  
- Energy efficiency in electric vehicles  
- Component of autonomous driving systems

---

## 🔮 Future Scope

- Integration of camera-based object classification (via OpenCV or ML)
- Use of fuzzy/PID control instead of threshold logic
- Vehicle-to-Vehicle (V2V) or V2I communication
- Sensor fusion (LiDAR, infrared)
- Cloud logging and real-time analytics

---



