# Laboratory Activity #5: Python-to-Arduino Serial Control

## Overview
This project shifts focus to software integration, using Python to send serial commands to the Arduino. A Python script serves as a controller interface, allowing a user to toggle LEDs on the Arduino board from their computer terminal.

## Objectives
- Implement Serial Connection between a computer (Python) and a microcontroller (Arduino).
- Create a Python script to act as a serial sender.

## Hardware Requirements
- Arduino MCU
- 3x LEDs (Red, Green, Blue)
- Laptop with Python & `pyserial` installed

## Pin Configuration
| Component | Pin |
|-----------|-----|
| Red LED   | 8   |
| Green LED | 9   |
| Blue LED  | 10  |

## Software Implementation
### Arduino Sketch
Listens for single-character serial inputs:
- `R`/`r`: Toggle Red LED
- `G`/`g`: Toggle Green LED
- `B`/`b`: Toggle Blue LED
- `A`/`a`: Turn All ON
- `O`/`o`: Turn All OFF

### Python Script
A non-terminating script that displays a menu and sends the corresponding characters to the Arduino port.
- Includes a "Clear Screen" feature for a clean UI.
- Inputs are case-insensitive.
- Pressing `X` terminates the Python program.
