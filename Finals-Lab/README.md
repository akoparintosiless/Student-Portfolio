# Final Exam: Arduino-to-Python API Client

## Overview
This final project requires the creation of a "Physical API Client." An Arduino with a push button acts as a trigger. When pressed, it signals a Python script, which then performs an actual HTTP Request to a remote API server. This demonstrates the decoupling of hardware triggers from network logic.

## Architecture
1. **Arduino (The Trigger):**
   - Monitors a Push Button.
   - Implements **Software Debouncing** to ensure clean signals.
   - Sends a specific "Group Number" via Serial when pressed.
   - *Constraint:* The Arduino does not make HTTP calls or control LEDs directly.

2. **Python Client (The Bridge):**
   - A non-terminating script listening to the Serial port.
   - Upon receiving the Group Number, it formats an HTTP request.
   - **Endpoint:** `GET /led/group/<number>/toggle`
   - Prints the API response (Success/Error) to the terminal.

## Key Constraints
- One physical button press must equal exactly one API request.
- Long presses must not spam the API.
- All Serial inputs are normalized/sanitized before use.
