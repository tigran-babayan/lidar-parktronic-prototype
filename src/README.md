# LiDAR Parktronic Prototype

A LiDAR-based proximity sensing system that provides real-time feedback
based on object distance.

This project demonstrates how distance sensors can be used to build
state-driven embedded systems for safety and awareness applications.

---

## Overview

The system continuously measures distance using a LiDAR sensor and
translates those measurements into clear feedback signals.

Based on proximity thresholds, the system updates LEDs, a buzzer,
and an LCD display to reflect the current distance state.

The focus of this project is reliable sensing, deterministic behavior,
and embedded control logic.

---

## Features

- Real-time distance measurement using LiDAR
- Multi-stage proximity states (safe → warning → critical)
- Visual feedback via LEDs
- Audible feedback via buzzer
- Live distance readout on LCD
- Deterministic, state-based logic
- Easily adjustable distance thresholds

---

## Proximity States

| State | Distance Range | Feedback |
|-----|---------------|----------|
| SAFE | Far | Green LED |
| WARNING | Medium | Yellow LED + slow buzzer |
| CRITICAL | Near | Red LED + fast buzzer |

State thresholds can be adjusted in code.

---

## System Architecture

LiDAR Sensor
↓
Arduino (distance processing + state logic)
↓
LEDs / Buzzer / LCD


Detailed architecture information can be found in `docs/architecture.md`.

---

## Hardware

- Arduino Uno
- LiDAR distance sensor (e.g. TF-Luna or similar)
- LEDs (green / yellow / red)
- Passive buzzer
- 16x2 LCD display
- Resistors and wiring

---

## Software

- Arduino IDE
- Embedded C++ (Arduino)

---

## Quick Start

1. Connect the hardware components (see `docs/wiring-and-pins.md`)
2. Open the Arduino sketch from the `src/` directory
3. Select **Board: Arduino Uno** and the correct COM port
4. Upload the sketch
5. Power the system and observe distance-based feedback

---

## Demo

A demo of the system behavior can be found in:
