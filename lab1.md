---
layout: project
title: Senior Design Lab 1
subtitle: Temperature Measurement System with Web Interface and SMS Alerts
permalink: /lab1/
---

## Introduction

The goal of this lab was to create a "third box" temperature measurement system that could be used independently as well as connected to the internet. The third box is a physically robust device that contains a temperature sensor, a display, a power switch, and a button to turn on the display. It can be used without internet, and the temperature will show on the display. When connected to internet, the temperature can be viewed as a graph on a web app. If the temperature goes above or below a threshold, an SMS alert will be sent to a specified phone number. The SMS alert and number can be changed from the web app.

## Design Process

- Attached waterproof temperature sensor to an embedded ESP32 microcontroller to continuously sample temperature
- Used ESP32's WiFi capabilities to transmit temperature data to the Internet
- Constructed a robust box for the hardware using a Tupperware container
- Displayed temperature data using a liquid crystal display (LCD)
- Implemented a web-based interface to:
    1. display real-time temperature and a graph of temperatures for the past 300s
    2. remotely turn the LCD screen on/off
    3. automatically send texts when temperature reaches a certain threshold

## Figures

![](/assets/img/Lab1ComDiagram.jpg)
*Figure 1: A diagram of major subsystems and communications between them*

![](/assets/img/lab1SDiagram.png)
*Figure 2: Schematic of circuit design of the third box*

![](/assets/img/Lab1_hardware.png)
*Figure 3: The complete project hardware, view of the interior*

## [Report](https://docs.google.com/document/d/1PQ9GbdkRLO2jWuFnlRnbq-0oBm3MXlaoVgIZr7sTr-U/edit?usp=sharing){:target="_blank"} -- [Code](https://github.com/accessdenied22/SeniorDesignLab1) -- [Web Interface](https://accessdenied.pythonanywhere.com/)
