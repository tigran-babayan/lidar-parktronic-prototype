# LiDAR Parktronic Prototype

## Overview
This project is a LiDAR-based proximity sensing prototype designed to explore system-driven behavior, real-time feedback, and hardware–software integration.

The system measures distance using a LiDAR sensor and reacts through visual, audio, and textual feedback depending on proximity thresholds. The goal of the project was not aesthetics, but understanding how sensing, logic, and output systems work together in a functional prototype.

---

## Key Features
- Real-time distance measurement using LiDAR
- State-based behavior depending on proximity
- Visual feedback via multi-stage LED indicators
- Audio feedback with variable alert patterns
- Distance display on a character LCD
- Designed and tested as a physical prototype

---

## System Behavior
The system operates in defined proximity states:

- **Safe zone** — Object far away  
  Green LED active, no sound

- **Warning zone** — Medium distance  
  Yellow LEDs activate progressively, slow audio alerts

- **Critical zone** — Very close distance  
  Red LED active with fast alert signal

This structure allows predictable and scalable system behavior.

---

## Demo

A short demo video demonstrating the system behavior:
https://www.youtube.com/watch?v=4142PttMiW8

---

## Hardware Components
- Arduino Uno
- TF-Luna LiDAR distance sensor
- Character LCD (parallel interface)
- LEDs (green, yellow, red)
- Passive buzzer
- Resistors and breadboard components

---

## Software
- Arduino C/C++
- State-based logic for distance thresholds
- Non-blocking timing for audio alerts
- Modular code structure for future expansion

---

## Development Notes
This prototype was developed through iterative testing:
- Hardware wiring and signal validation
- Sensor data stabilization
- Threshold tuning for smooth transitions
- Output synchronization across LEDs, audio, and display

The project emphasizes system thinking and hands-on experimentation rather than polished enclosure design.

---

## Future Improvements
- Enclosure / product casing
- Noise filtering and signal smoothing
- Adjustable thresholds via user input
- Migration to a more compact microcontroller
- Power optimization

---

## Author
**Tigran Babayan**  
Creative Technologist — Product & Hardware Prototyping
