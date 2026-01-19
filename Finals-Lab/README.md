Problem Statement

Design a system where an Arduino button triggers a signal to a Python program that calls an external API to control remote hardware.

Requirements Summary

Arduino:

- Detect button press with debouncing

- Send signal group number once per press

Python Client:

- Listen on serial port

- On valid signal, call:

/led/group/<number>/toggle

= /led/group/<number>/toggle

Rules

- One button press → one API request

- Long presses do NOT trigger multiple calls

- Handle input errors gracefully
