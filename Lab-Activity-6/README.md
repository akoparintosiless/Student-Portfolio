Laboratory Activity #6 — Bidirectional Arduino & Python

Objectives

- Implement bidirectional serial communication between Arduino and Python.

Description

Arduino reads push button events and sends signals to Python. Python then sends back commands to toggle LEDs on Arduino.

Components

- Arduino, 3 LEDs, 3 Buttons

LED pins:

- Red: 7

- Green: 6

- Blue: 5

Button pins:

- Button 1: 12

- Button 2: 11

- Button 3: 10

Logic

Arduino: Outbound

- Button1 → “R”

- Button2 → “G”

- Button3 → “B”

Arduino: Inbound

- Received “1” → toggle Red

- Received “2” → toggle Green

- Received “3” → toggle Blue

Python:

- Sends “1”, “2”, “3” back based on button characters

- Ensures under 1 second response
