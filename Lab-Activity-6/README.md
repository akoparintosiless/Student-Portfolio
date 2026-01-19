# Laboratory Activity #6: Bidirectional Arduino-Python Communication

## Overview
This activity implements full bidirectional communication. The Arduino sends data to Python when buttons are pressed, and Python sends commands back to the Arduino to control LEDs. This simulates a responsive IoT loop.

## Objectives
- Implement bidirectional Serial communication.
- Synchronize inputs and outputs between two different programming environments.

## Hardware Requirements
- Arduino MCU
- 3x LEDs (Red, Green, Blue)
- 3x Push Buttons
- Python environment

## Pin Configuration
| Component | Pin | Component | Pin |
|-----------|-----|-----------|-----|
| Blue LED  | 5   | Button 3  | 10  |
| Green LED | 6   | Button 2  | 11  |
| Red LED   | 7   | Button 1  | 12  |

## System Workflow
1. **Arduino (Outbound):** - Pressing Button 1/2/3 sends the character `R`/`G`/`B` to Python via Serial.
   - The Arduino does **not** turn on the LEDs locally.
2. **Python (Processing):** - Listens for `R`, `G`, or `B`.
   - When received, it sends a numeric command back to Arduino (`1`, `2`, or `3`).
3. **Arduino (Inbound):** - Receives `1`: Toggles Red LED.
   - Receives `2`: Toggles Green LED.
   - Receives `3`: Toggles Blue LED.
