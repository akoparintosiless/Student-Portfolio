Laboratory Activity #3 — Working with Sensors

Objectives

- Learn basic sensor components for IoT.

- Integrate sensors in an Arduino circuit.

- Implement a simple fire detection simulation.

Description

This project uses a thermistor and a photoresistor to detect heat and brightness, respectively.

Circuit Details

- Thermistor → A0

- Photoresistor → A2

- Red LED (fire indicator) → Digital pin 12

Threshold Logic

- Temperature in Celsius and light intensity threshold monitored.

  - Thresholds:

  - Temp ≥ 50°C

- Brightness ≤ 220

- If both thresholds are met → fast blinking LED.

Optional buzzer connected to same pin for audible alert.
