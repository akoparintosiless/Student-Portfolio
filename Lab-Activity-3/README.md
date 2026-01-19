# Laboratory Activity #3: Working with Sensors (Fire Detector)

## Overview
This project focuses on integrating sensors into an IoT system. We create a basic "Fire Sensor" system that monitors temperature and light levels to detect potential fire hazards.

## Objectives
- Familiarize with basic sensor components (Thermistor & Photoresistor).
- Integrate analog sensors into an Arduino circuit.
- Create a logic-based alarm system.

## Hardware Requirements
- Arduino MCU
- Thermistor (Temperature Sensor)
- Photoresistor (Light Sensor)
- Red LED
- Buzzer/Speaker (Optional)
- Resistors (10kΩ for sensors, 220Ω for LED)

## Pin Configuration
| Component      | Pin Type | Pin Number |
|----------------|----------|------------|
| Thermistor     | Analog   | A0         |
| Photoresistor  | Analog   | A2         |
| Red LED        | Digital  | 12         |
| Buzzer         | Digital  | 12         |

## Program Logic
The system reads analog data from both sensors and converts it to readable values (Celsius for temperature, raw digital value for light).
- **Thresholds:**
  - Temperature: > 50°C
  - Brightness: > 220
- **Alarm Condition:** If **BOTH** thresholds are met simultaneously (High Temp AND High Light), the system triggers the alarm.
- **Alarm Action:** The Red LED (and optional buzzer) blinks rapidly to indicate a fire warning.
