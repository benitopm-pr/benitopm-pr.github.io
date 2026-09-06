---
layout: project
title: "Milky Way Detection via Hydrogen Density (DSP)"
description: "Digital Signal Processing project: detecting the Milky Way's position using hydrogen emission frequency data, with a custom helical antenna and a motorized mechanical pointing system."
date: 2023-01-01
categories: [Digital Signal Processing, RF/Antennas, Mechatronics]
components:
  - name: "Helical antenna"
    quantity: 1
    description: "Custom-built, tuned to the hydrogen emission frequency (21cm line)"
  - name: "Stepper motor (892-8732)"
    quantity: 1
    description: "Selected for the antenna's mechanical pointing/tracking system"
  - name: "Cycloidal gearing"
    quantity: 1
    description: "Chosen for high torque, minimal backlash, and high efficiency when lubricated"
---

## Project Overview

A university Digital Signal Processing project: detecting the Milky Way's position by measuring hydrogen emission density using a custom-built helical antenna, then processing real sky survey data (FITS files) to output a heatmap of the galaxy's position. The team built and used a real antenna for this project.

**Capabilities:**
- Reading, segmenting, and splitting FITS data from sky surveys
- Filtering for the hydrogen emission frequency, then interpreting and outputting a heatmap showing the Milky Way's position relative to the original survey image

## Team & My Role

This was a team project. **I was in charge of the antenna's mechanical pointing/tracking system** — the motorized system intended to aim the antenna toward a target celestial object. My work included:

- **Requirements definition:** Established the key requirements for the pointing mechanism — high precision, minimal vibration, and low backlash
- **Gear selection:** Evaluated gear types and selected cycloidal gearing for its high torque, near-zero backlash, and high efficiency when well lubricated
- **Motor selection:** Selected the stepper motor (892-8732) for the system, after comparing it against alternative options
- **Mathematical modeling (MATLAB):** Calculated the telescope/antenna beamwidth, tracking position, gear ratios, number of gear stages, required torque, and weight capacity

## Skills Demonstrated

- RF/antenna fundamentals (hydrogen line detection)
- FITS astronomical data processing
- Mechanical drivetrain design (gear selection, torque/backlash trade-offs)
- MATLAB-based engineering calculations
- Motor selection based on system requirements