# Laboratory Activity #2: Working with Analog Signals

## Overview
This activity expands on the previous running light circuit by introducing analog signals. Instead of simply turning LEDs on and off, this project controls the brightness of the LEDs using Pulse Width Modulation (PWM), demonstrating the difference between digital and analog output.

## Objectives
- Discuss analog signals and their implementation in an Arduino circuit.
- Understand analog-to-digital signal conversion.
- Utilize the `map()` function and `analogWrite()`.

## Hardware Requirements
- Arduino MCU
- 5x LEDs
- Resistors
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
The code logic mirrors Activity #1 but utilizes `analogWrite()` for brightness control.
- **Looping:** Implemented using `while()` loops and arrays for pin management.
- **Sequence:** Running light pattern from Pin 12 to Pin 8.
- **Behavior:** LEDs fade/activate sequentially with a 1-second delay, demonstrating analog control over digital pins.
