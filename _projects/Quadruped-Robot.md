---
layout: project
title: "Quadruped Robot"
description: "A self-built quadruped robot (Boston Dynamics Spot-inspired), combining embedded firmware and ROS2 for full-stack robotics learning."
date: 2026-09-06
categories: [Robotics, Embedded Systems, ROS2, Mechatronics]
github_url: "https://github.com/benitopm-pr/quadruped-robot"

components:
  - name: "High-torque digital RC servos"
    quantity: 12
    description: "20-35 kg·cm range, metal gears, PWM signal, driving each leg joint"
  - name: "PCA9685 PWM driver"
    quantity: 1
    description: "16-channel I2C PWM driver for servo control"
  - name: "ATmega-based microcontroller (PlatformIO)"
    quantity: 1
    description: "Low-level real-time motor control firmware, written in C"
  - name: "Raspberry Pi 5"
    quantity: 1
    description: "High-level compute for ROS2: gait generation, inverse kinematics, control logic"
  - name: "Bosytro DY-12V600W power supply"
    quantity: 1
    description: "Adjustable 0-13.2V, 50A max, 600W"
  - name: "3D printer"
    quantity: 1
    description: "Used to print the leg and chassis structural parts"
---

## Project Overview

A self-directed project to design and build a quadruped robot, inspired by Boston Dynamics' Spot. The goal is hands-on, practical experience across mechanics, electronics, embedded firmware, and control engineering — extending beyond university coursework.

## Architecture

The robot follows a two-tier control architecture, mirroring how real-world robotics systems are typically structured:

- **Low-level tier:** An ATmega-based microcontroller (programmed in C via PlatformIO) handles real-time actuation — driving the servos through a PCA9685 PWM driver.
- **High-level tier:** A Raspberry Pi 5 runs ROS2, handling gait generation, inverse kinematics, and higher-level control logic, communicating with the microcontroller over serial.

## Current Status

The project is in progress. The mechanical design is being modeled in SolidWorks, and the electronics (servos, PCA9685, power supply) and compute hardware (Raspberry Pi 5) are in hand. Firmware and ROS2 integration are the next steps.

## Skills Demonstrated

- Embedded C firmware development (PlatformIO)
- CAD design (SolidWorks)
- ROS2 (in progress)
- Full-stack robotics system architecture