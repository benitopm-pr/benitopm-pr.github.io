---
layout: project
title: "Quadcopter Drone — 4th Semester Project"
description: "4th semester mechatronics team project: a quadcopter drone built around a BeagleBone Blue flight computer, achieving stable hover in test flights."
date: 2024-05-14
categories: [Robotics, Drones, Control, Embedded Systems]
components:
  - name: "BeagleBone Blue"
    quantity: 1
    description: "Flight computer, running IMU-based sensing and control"
  - name: "IMU (accelerometer + gyroscope)"
    quantity: 1
    description: "Onboard the BeagleBone Blue; integrated over I2C"
  - name: "Height sensor"
    quantity: 1
    description: "Evaluated barometric, ultrasonic, and time-of-flight options for altitude sensing"
---

## Project Overview

A 4th semester mechatronics team project (SDU, Feb–May 2024), built by a 6-person team (Group IX): Benito Padilla, Daniel, Dimitris, Eduard, Kenneth, and Marius. The goal was to design, build, and fly a quadcopter drone capable of stable hover, with a strong focus on control engineering. The drone completed test flights in May 2024.

## Team & My Role

The team assigned leadership areas per discipline; **I was the team's Electronics Lead**, responsible for:

- **Electrical schematic:** Finalized the drone's electrical schematic once the team's parts list was complete
- **Sensor integration:** Worked with a teammate on integrating the IMU (accelerometer + gyroscope) via the BeagleBone Blue, troubleshooting I2C communication issues
- **Height sensing evaluation:** Contributed to evaluating altitude-sensing options (barometric, ultrasonic, and time-of-flight sensors) for the drone's height control
- **Risk assessment:** Authored the risk assessment section of the final report

## Skills Demonstrated

- Electrical schematic design for a multi-subsystem embedded system
- I2C sensor integration and debugging
- Sensor selection and trade-off evaluation
- Team leadership (Electronics domain) in a 6-person cross-disciplinary project