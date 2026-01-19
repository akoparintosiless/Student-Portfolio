# Midterm Exam: Smart Lighting System

## Overview
The Smart Lighting System is an environment-aware project that adjusts LED indicators based on ambient light intensity. It features both a **Manual Mode** (where users set thresholds) and an **Automatic Mode** (where the system simulates responses to weather conditions).

## Hardware Requirements
- Arduino MCU
- Photoresistor (Light Sensor)
- 3x LEDs (Green, Yellow, Red)

## System Logic
**Light Intensity Mapping:** - Sensor reads 0-1023 and maps it to 0-100%.

**LED Status Indicators:**
- **Green:** Low Light Intensity
- **Yellow:** Medium Light Intensity
- **Red:** High Light Intensity

**Modes of Operation:**
1. **Automatic Mode (`MODE AUTO`):** - Thresholds adjust dynamically to simulate weather:
     - *Cloudy:* Low (0-40%), High (40%+)
     - *Normal:* Low (41-70%), High (70%+)
     - *Bright Sunlight:* Low (71-100%)
2. **Manual Mode (`MODE MANUAL`):**
   - User can define custom thresholds via Serial commands:
     - `SET LOW xx`
     - `SET HIGH xx`

**Serial Output:**
Updates every second with:
- Light Intensity %
- Active LED
- Current Mode
