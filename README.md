# Maze-solving-line-follower-robot
Developed an Arduino-based autonomous robot that detects and follows a predefined path using IR sensors. Implemented motor control using an L293D motor driver and programmed sensor-based movement logic to automatically move forward, turn left/right, and stop according to the detected line.

# Line Following Robot

This project is an Arduino-based line-following robot using IR sensors and an L293D motor driver.

## 🔧 Components Used

- Arduino Uno (or compatible)
- L293D Motor Driver
- IR Sensors (Left and Right)
- DC Motors (2)
- Wheels and Chassis
- Jumper Wires
- Power Supply (Battery/USB)

## ⚙️ Pin Configuration

| Component     | Arduino Pin |
|---------------|-------------|
| Left Sensor   | D10         |
| Right Sensor  | D9          |
| Left Motor IN1| D7          |
| Left Motor IN2| D6          |
| Right Motor IN3| D5         |
| Right Motor IN4| D4         |
| Left Motor PWM| D3 (ENA)    |
| Right Motor PWM| D11 (ENB)  |

## 🚦 How It Works

- **Both Sensors White (0 0)**: Move Forward
- **Left Black, Right White (1 0)**: Turn Left
- **Left White, Right Black (0 1)**: Turn Right
- **Both Black (1 1)**: Stop

## 💾 Code

The main logic is written in Arduino C (`main.ino`). Adjust `analogWrite` values to tune speed for your setup.

## 📁 File Structure

```
line_following_robot/
├── main.ino
└── README.md
```

## 🧠 Author

Created by Gobinath  
For academic and robotics learning purposes.
