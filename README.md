# 👁️‍🗨️ Gaze- & Gesture-Controlled Wheelchair

Vision-based wheelchair control system using **eye-gaze tracking** and **hand gesture recognition**.

---

## 📌 Overview

This project explores a **computer-vision-based interaction system** for controlling an electric wheelchair using eye movements and hand gestures.  
The system aims to improve accessibility for users with severe motor impairments by reducing reliance on traditional physical input devices.

The project was developed between **January 2022 and September 2022** as an **independent research and engineering project**, focusing on system design, feasibility analysis, and experimental validation of vision-based assistive control.

---

## 🎯 Motivation

Individuals with motor disorders or endocrine-related conditions such as **acromegaly** may experience progressive loss of fine motor control.  
In advanced cases, **eye movement can remain one of the most reliable voluntary control signals**.

This project investigates whether **eye-gaze direction** can be used as a primary control input, with **hand gestures** serving as a supplementary and safety-oriented mechanism for wheelchair navigation.

---

## 🧠 System Design

The proposed system consists of three main components:

### 1️⃣ Eye-Gaze Tracking Module
- Captures eye images using a standard camera
- Extracts and analyzes the eye region
- Estimates gaze direction by measuring the **relative sclera (white region) ratio**
- Maps gaze direction to movement commands:
  - Center → move forward  
  - Left → turn left  
  - Right → turn right  

Gaze ratios from both eyes are averaged to improve stability and reduce individual bias.

---

### 2️⃣ Hand Gesture Recognition Module
- Uses camera-based hand detection
- Recognizes predefined body and hand gestures
- Acts as a confirmation and redundancy layer to reduce accidental activation

---

### 3️⃣ Control & Communication Layer
- Integrates gaze and gesture signals
- Sends commands from a computer to a microcontroller
- Drives left and right motors via an H-bridge motor controller

---

## 🧪 Experimental Results

- Successful real-time detection of gaze direction under controlled lighting conditions
- Wheelchair movement commands (forward, left, right, stop) generated from visual input
- Gesture-based control improved reliability and user confidence

**Key observations:**
- The system significantly reduces hardware cost (only a camera and computer required)
- Per-user calibration is necessary due to individual eye characteristics
- Performance is sensitive to lighting conditions and prolonged usage

---

## 🏅 Awards & Recognition

- 🥇 **Gold Medal**, INNOVERSE EXPO (USA)  
- 🥇 **Gold Medal**, 1 Idea 1 World Invention Competition (Turkey)

The project was presented under the title:  
**“Intelligent Wheelchair for Patients with Acromegaly”**

---

## ⚠️ Notes on Implementation

- The original implementation was experimental and hardware-dependent
- The complete runnable source code is **no longer fully preserved**
- This repository serves as **project documentation and portfolio evidence**, highlighting system design, methodology, and results rather than a production-ready software release

---

## 📄 Project Report

📘 **Full technical report (PDF):**  
👉 https://github.com/vascosio1114/gaze-gesture-controlled-wheelchair/blob/main/gaze-gesture-controlled-wheelchair-report.pdf

The report includes:
- Background research and motivation  
- System architecture and diagrams  
- Mathematical formulation of gaze ratio calculation  
- Experimental setup and evaluation  
- Discussion of limitations  

---

## 👤 Author

**Kei Chon Sio**  
Interests: Data Analytics, Python, Computer Vision, Accessibility Technology  

📫 Contact: keichonsio1114@gmail.com

---

## 📜 License

This project is licensed under the **MIT License**.
