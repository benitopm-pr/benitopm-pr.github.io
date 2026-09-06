---
layout: project
title: "SPRO-1 — Rally Car"
description: "1st semester mechatronics team project: a microcontroller-driven car that drives a user-specified distance in a user-specified time, with real-time display, motor control, and safety monitoring."
date: 2023-01-15
categories: [Mechatronics, Embedded Systems, Arduino]
github_url: "https://github.com/Hoprap54/1_Semester_Project"

components:
  - name: "Arduino Nano"
    quantity: 1
    description: "Main microcontroller"
  - name: "Nextion touchscreen display"
    quantity: 1
    description: "User input (distance/time per stage) and real-time status display"
  - name: "L298N motor driver"
    quantity: 1
    description: "Dual full-bridge driver for motor speed and direction control"
  - name: "Optocoupler + encoder wheel"
    quantity: 1
    description: "Interrupt-driven speed and distance tracking"
  - name: "LM7805 voltage regulator"
    quantity: 1
    description: "Power circuit stabilization"

gallery:
  - type: "video"
    file: "/assets/images/projects/sprog1-rally-car/demo.mp4"
    description: "Rally car demo"
---

## Project Overview

A 1st semester mechatronics project (SDU, Sep 2022 – Jan 2023), built by a 6-person team (5 Mechatronics students, 1 Mechanical student): Henrik, Benito, Zosia, Miro, Abdullah, and Tobiloba.

The car had to:
- Drive a user-specified distance in a user-specified time
- Take input from and display real-time information on a Nextion touchscreen
- Measure battery voltage and stop automatically if it dropped too low
- Indicate acceleration/braking and driving direction via LEDs
- Include a path line-marking mechanism
- Measure and display counter-torque

## Team & My Role

This was a team project — the mechanical base and wheel adapter concepts were originally designed by teammate Zosia. My specific contributions were:

- **Mechanical design:** Adapted the base plate size and added component mounting holes; modified the wheel adapter (enlarged the back section, added a hole to improve shaft grip)
- **Enclosure design:** Designed the electronics box housing the mainboard, battery, and display, with cable routing
- **Electrical design:** Contributed to the circuit schematic, including adding a power switch and the voltage divider circuit used to measure battery voltage via the ADC
- **Embedded firmware:** Worked with teammate Henrik on the motor control code — configured Fast PWM on the L298N driver, with autoregulated speed control to meet the user-specified distance/time
- **Extra feature:** Implemented the front LED lights, which activate when the car is in a driving stage and moving forward

## Skills Demonstrated

- Embedded C programming (AVR registers, Fast PWM, interrupts)
- CAD design and iteration (NX)
- Electronics: voltage regulation, voltage dividers, ADC-based battery monitoring
- Team-based mechatronics development workflow