---
layout: project
title: Senior Design Lab 2
subtitle: Noise-Robust Infrared Light Curtain Receiver with Buzzer and SMS Alerts
permalink: /lab2/
---

## Introduction

The goal of this lab was to create a receiver that would detect an infrared signal from a transmitter provided. This receiver must be robust in the presence of noise, such as sunlight or ambient light from incandescent bulbs. The receiver is meant to function like a "light curtain" in that it should detect if the infrared beam is broken. If the beam is broken, a buzzer should sound and an SMS alert should be sent to a hard-coded phone number.

## Design Process

- Analyzed provided transmitter to determine characteristics of the infrared signal
- Inspected many operational amplifier (op amp) datasheets to design and create a 2nd order Butterworth high pass filter using a Sallen-Key topology
- Designed circuit layout with components incl. infrared phototransistor, buffer, filter, amplifier, and voltage regulator
- Read voltage output from the receiver using the analog-to-digital converter (ADC) in Arduino Uno with C++
- Implemented logic to detect beam obstruction using Arduino Uno C++
- Connected Arduino to a computer using serial USB, then used a Python script on computer to send SMS alerts

## Figures

![](/assets/img/Lab2ComDiagram-2.jpg)
*Figure 1: A high-level view of major subsystems*

![](/assets/img/Lab2_circuit.png)
*Figure 2: Schematic of circuit design*

![](/assets/img/sd_lab2_sq.jpg)
*Figure 3: The complete receiver circuit*

## [Report](https://docs.google.com/document/d/1aG0b_mFECTtD6Mjk1xTKgTgyh8bTG4-WC5oXn0yhgpk/edit?usp=sharing){:target="_blank"} -- [Code](https://github.com/accessdenied22/SeniorDesignLab2)
