Problem Statement

Build a smart outdoor lighting system using Arduino and a photoresistor to indicate light levels automatically and manually.

🧠 Features

Convert sensor reading to % (0–100)

Use three LEDs to show:

Low → Green

Mid → Yellow

High → Red

User Commands (Serial)

| Command       | Action             |
| ------------- | ------------------ |
| `MODE AUTO`   | Automatic Mode     |
| `MODE MANUAL` | Manual Mode        |
| `SET LOW xx`  | Set low threshold  |
| `SET HIGH xx` | Set high threshold |

Automatic Mode

| Condition       | Thresholds             |
| --------------- | ---------------------- |
| Cloudy          | Low = 0%, High = 40%   |
| Normal          | Low = 41%, High = 70%  |
| Bright Sunlight | Low = 71%, High = 100% |

