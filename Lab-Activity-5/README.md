Laboratory Activity #5 — Arduino & Python Serial Connection
Objectives

- Implement Arduino Serial connection.

- Use Python to control Arduino via serial communication.

Description

This lab demonstrates sending commands from Python to Arduino to control LEDs.

Components

- Arduino

- 3 LEDs (Red:8, Green:9, Blue:10)

- Breadboard, resistors, wires

Serial Logic

Arduino listens for serial inputs:

 Input	  /    Action
- R/r	   /   Toggle Red LED
- G/g	   /   Toggle Green LED
- B/b	   /   Toggle Blue LED
- A/a	   /   All LEDs ON
- O/o	   /   All LEDs OFF
- Other	 /   Send error

Python Script

- Runs indefinitely showing menu

- User chooses commands:

[R] Red ON/OFF
[G] Green ON/OFF
[B] Blue ON/OFF
[A] All ON
[O] All OFF
[X] Exit
