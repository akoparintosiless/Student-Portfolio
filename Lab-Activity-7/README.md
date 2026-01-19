# Laboratory Activity #7: Web-Based Control using FastAPI

## Overview
This project modernizes the serial controller by wrapping the Python logic in a FastAPI web server. Instead of a terminal menu, the Arduino is controlled via HTTP API endpoints, simulating a cloud-connected IoT device.

## Objectives
- Implement an HTTP-based solution for IoT control.
- Bridge a REST API (FastAPI) with Hardware Serial communication.

## Hardware Requirements
- Arduino MCU
- 3x LEDs (Red, Green, Blue)
- 3x Push Buttons

## Pin Configuration
*Same layout as Activity #6*
- **LEDs:** Red (7), Green (6), Blue (5)
- **Buttons:** B1 (12), B2 (11), B3 (10)

## API Endpoints
The Python script hosts a local server providing the following routes:

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/led/red` | Sends signal "1" to Arduino (Red LED) |
| GET | `/led/green` | Sends signal "2" to Arduino (Green LED) |
| GET | `/led/blue` | Sends signal "3" to Arduino (Blue LED) |
| GET | `/led/on` | Turns all LEDs ON |
| GET | `/led/off` | Turns all LEDs OFF |
