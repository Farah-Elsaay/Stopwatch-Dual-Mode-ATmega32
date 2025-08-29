# ⏱️ Stopwatch with Dual Mode (Increment & Countdown)

## 📌 Project Overview
A digital stopwatch system built using **ATmega32 microcontroller** and **six multiplexed seven-segment displays**, supporting two operational modes:

- 🔺 **Increment Mode (Default):** Counts up from zero.  
- 🔻 **Countdown Mode:** Counts down from a user-defined time and triggers a **buzzer alarm** when it reaches zero.  

This project demonstrates **embedded systems design**, **real-time processing**, and **hardware-software integration** using C and FreeRTOS.

---

## ✨ Features
- ⏱️ Stopwatch with **Increment & Countdown modes**  
- ⏸️ **Pause / Resume / Reset** functions  
- 🔔 **Buzzer alarm** when countdown finishes  
- 💡 **LED indicators** for active mode  
- 🔄 **User time adjustment** (hours, minutes, seconds) via push buttons  
- ⚡ **Multiplexed seven-segment display** for efficient hardware usage  

---

## 🛠️ Hardware Components
- **Microcontroller:** ATmega32  
- **Displays:** 6x seven-segment displays (common anode)  
- **Decoder:** 7447 BCD-to-7-segment decoder  
- **Input:** 10 push buttons (reset, pause, resume, toggle, time adjust)  
- **Alarm:** Buzzer (countdown complete)  
- **Indicators:** Red LED (increment mode), Yellow LED (countdown mode)  

---

## ⚙️ System Design
- **MCU Frequency:** 16 MHz  
- **Timer1:** Configured in **CTC mode** for stopwatch timing  
- **Interrupts:**


  - `INT0` → Reset  
  - `INT1` → Pause  
  - `INT2` → Resume  
- **Multiplexing:** One display active at a time using transistors + persistence of vision  
- **Mode Control:** Toggle button for increment ↔ countdown  

---

## 🎥 Demo
📹 [Watch the project in action](https://youtu.be/-7c2NCQg5r4)

---

---

## 🧠 Skills Demonstrated
- Embedded Systems Design  
- Microcontrollers (ATmega32, AVR architecture)  
- FreeRTOS & Real-Time Programming  
- C Programming & Firmware Development  
- Digital Electronics & Circuit Design  
- Timer/Counter Configuration  
- Interrupt Handling  
- Seven-Segment Multiplexing  
- Hardware Debugging (Oscilloscope / Logic Analyzer)  

---

## 🚀 Future Improvements
- Add **real-time clock (RTC) module** for extended timing accuracy  
- Add **EEPROM save function** to store countdown presets  
- Extend design to support **lap-time functionality**  
- Implement on **LCD / OLED** for improved display  

---

## 👨‍💻 Author
Developed as part of the **Standard Embedded Diploma - Mini Project 2** by Farah Elsaay.  
