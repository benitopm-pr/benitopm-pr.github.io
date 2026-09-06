---
layout: project
title: "CNC Mill Machine"
description: "2nd semester mechatronics team project: a CNC milling machine with stepper-driven XY-table, G-code interpretation, manual D-pad control, and limit-switch-based auto-calibration."
date: 2023-06-01
categories: [Mechatronics, CNC, Embedded Systems, Electronics]
components:
  - name: "Arduino Nano (ATmega328P) x2"
    quantity: 2
    description: "Split across two boards due to pin count requirements"
  - name: "L298N motor driver"
    quantity: 5
    description: "Dual H-bridge driver per stepper motor, bipolar configuration for higher torque"
  - name: "Hybrid stepper motors"
    quantity: 5
    description: "6V, 1.25A/0.85A depending on axis, driving the XY-table"
  - name: "Limit switches"
    quantity: "multiple"
    description: "Used for auto-calibration and to prevent the mill from over-traveling"
  - name: "Custom D-pad controller"
    quantity: 1
    description: "7-button resistor-ladder controller read via ADC, for manual axis control"
  - name: "7809 voltage regulators"
    quantity: 3
    description: "Wired in parallel to supply 9V/6A to the motor rail"
---

## Project Overview

A 2nd semester mechatronics team project (SDU, completed June 2023), built by a 5-person team: Benito Padilla, Christian Berg Christensen, Daniel Borregaard, Dimitris Kralidis, and Marius Tilea. The goal was to design and build a working CNC milling machine capable of G-code interpretation, manual control, and safe autonomous operation.

## Team & My Role

This was a team project spanning mechanical, electrical, and software design. **My contribution was the entire electrical design:**

- **Motor drivers:** Selected and specified 5x L298N motor drivers, matched to the stepper motors' electrical specs (6V, 1.25A)
- **Stepper motor configuration:** Analyzed unipolar vs. bipolar stepper motor theory and chose a bipolar configuration to maximize torque, leveraging the L298N's built-in dual H-bridges
- **Drill control circuit:** Designed the drill on/off switching circuit using an NPN transistor with a flyback diode for residual current, isolated from the microcontroller circuit via an optocoupler
- **Microcontroller selection:** Chose 2x Arduino Nano (ATmega328P) to work around pin-count limitations, keeping a known/familiar microcontroller family
- **D-pad controller:** Designed a custom 7-button manual controller using a resistor-ladder configuration, read via ADC, allowing simultaneous button presses across axes
- **Sensor selection:** Selected limit switches for auto-calibration and travel-limit safety, after evaluating (and ruling out, due to budget) hall-effect rotary encoders
- **Power budget & supply:** Calculated total system current draw across motors, microcontrollers, SD card reader, and controller, and selected a 12V/6A power supply; designed a 3x parallel 7809 voltage regulator board to deliver the required 9V motor rail

## Skills Demonstrated

- Motor driver and H-bridge circuit design
- Stepper motor theory (unipolar/bipolar tradeoffs)
- Power budgeting and regulator design
- Sensor selection for safety-critical auto-calibration
- Embedded electronics (ATmega328P-based systems)