# Laboratory Activity #4: Arduino Serial Connection

## Overview
This activity explores the Serial Communication capabilities of the Arduino. Using the sensor circuit from Activity #3, we implement a control system that can send data to the Serial Monitor and receive text commands to control the hardware.

## Objectives
- Understand and implement Arduino Serial Connection.
- Control a circuit remotely using Serial commands.

## Hardware Requirements
- Arduino MCU
- Sensor (Thermistor OR Photoresistor)
- LED
- Resistors

## Pin Configuration
| Component | Pin |
|-----------|-----|
| Sensor    | A0 or A2 |
| LED       | 8   |

## Program Logic
1. **Monitoring:** The system continuously monitors the chosen sensor.
   - *Thermistor Threshold:* 50°C
   - *Photoresistor Threshold:* 220
2. **Trigger:** If the sensor reading exceeds the threshold, the LED on Pin 8 begins blinking (Delay: 100ms).
3. **Latching:** The blinking continues **even if the sensor reading drops back down**.
4. **Manual Override:** The blinking stops **only** when the user types the word `"stop"` (case-insensitive) into the Serial Monitor.
