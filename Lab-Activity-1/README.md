# Laboratory Activity #1: Working with Digital Signals

## Overview
This activity introduces the Arduino as a tool for IoT systems by focusing on digital signal implementation. The project involves creating a "Running Light" circuit where LEDs turn on and off in a sequential pattern using digital outputs.

## Objectives
- Review Arduino as a device for IoT systems implementation.
- Discuss and demonstrate digital signals in an Arduino circuit.

## Hardware Requirements
- Arduino MCU
- 5x LEDs
- Resistors (220Ω or 330Ω)
- Breadboard and Jumper Wires

## Pin Configuration
| Component | Pin |
|-----------|-----|
| LED 1     | 12  |
| LED 2     | 11  |
| LED 3     | 10  |
| LED 4     | 9   |
| LED 5     | 8   |

## Program Logic
The firmware utilizes `digitalWrite()` to control the state of the LEDs.
1. **Sequence:** The LEDs light up sequentially from Pin 12 to Pin 8.
2. **Behavior:** - All LEDs turn **ON** one by one.
   - All LEDs turn **OFF** one by one.
   - **Delay:** 1 second between each state change.
