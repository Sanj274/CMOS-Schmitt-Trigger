# CMOS Schmitt Trigger (Low-Power Hysteresis Comparator)

## Overview
This project presents the design and simulation of a CMOS Schmitt Trigger implemented in Cadence Virtuoso using gpdk90 technology.  
The circuit is designed to provide strong noise immunity and stable switching behavior through controlled hysteresis. It functions as a low-power hysteresis comparator suitable for signal conditioning and waveform shaping applications.

---

## Objective
To design a CMOS-based Schmitt Trigger with:
- Reliable hysteresis characteristics
- Stable switching thresholds
- Improved noise immunity
- Low power consumption

  <img width="2560" height="1358" alt="image" src="https://github.com/user-attachments/assets/8a56fb05-aed9-4591-8e0d-d1c22a538394" />


---

## Design Concept

A Schmitt Trigger introduces two distinct switching thresholds:
- Upper Threshold Voltage (Vth+)
- Lower Threshold Voltage (Vth−)

  <img width="1000" height="470" alt="image" src="https://github.com/user-attachments/assets/67f4ff16-7e6f-4bbe-9ad1-79b72342242d" />


This hysteresis prevents false triggering caused by noise or slow input transitions.

The design uses:
- CMOS pull-up and pull-down transistor networks
- Positive feedback mechanism
- Optimized transistor sizing to control hysteresis width

---

## Design Methodology

### 1. Transistor Sizing Optimization
Transistor dimensions were carefully adjusted to:
- Control switching thresholds
- Achieve desired hysteresis width
- Maintain stable operation across input variations

### 2. Positive Feedback Implementation
Feedback paths were introduced to create distinct rising and falling transition points.

### 3. Supply Voltage
- VDD: 1.8V

  <img width="886" height="773" alt="schematic" src="https://github.com/user-attachments/assets/e5a3b998-948a-4615-8e1c-0222f1250e55" />


---

## Simulation Setup

- Tool: Cadence Virtuoso
- Technology: gpdk90
- Analysis Type: Transient Analysis
- Input: Time-varying analog signal (sine/ramp)
- Output: Digital square waveform

Transient simulations were performed to verify:
- Clean switching behavior
- Proper hysteresis window
- Noise immunity
- Stable output transitions

---

## Results

The simulated results demonstrate:

- Clear hysteresis behavior
- Stable switching points
- Noise-resistant output transitions
- Proper square wave generation from analog input

  <img width="1465" height="616" alt="output1" src="https://github.com/user-attachments/assets/ae00dd0c-33dc-4442-8458-c825777e6110" />

  <img width="1460" height="622" alt="output2" src="https://github.com/user-attachments/assets/2689d65a-4be3-496d-9970-98a6095b7060" />


The output waveform confirms distinct threshold voltages for rising and falling edges, validating correct Schmitt Trigger functionality.

---

## Key Features

- CMOS-based low-power design
- Improved switching stability
- Enhanced noise immunity
- Suitable for analog-to-digital interfacing
- Efficient comparator structure

---

## Applications

- Signal conditioning circuits
- Waveform shaping
- Noise filtering
- Analog-to-digital front-end circuits
- Oscillator and timing circuits

---

## Tools & Technologies

- Cadence Virtuoso
- gpdk90
- CMOS Analog Design
- Transient Simulation (ADE L)

---
