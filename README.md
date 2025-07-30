# Autonomous-Obstacle-Avoidance-Car-using-Arduino
An Arduino-powered smart car with 4 DC motors, a servo motor, and an ultrasonic sensor. It detects and avoids obstacles automatically using distance sensing and motor control with the L293D motor driver shield.

# Components Used

| Component                 | Description                                 |
| ------------------------- | ------------------------------------------- |
| Arduino UNO               | Main microcontroller                        |
| L293D Motor Driver Shield | Controls 4 DC motors via Arduino            |
| 4x DC Motors              | For 4-wheel drive motion                    |
| HC-SR04 Ultrasonic Sensor | Measures distance to obstacles              |
| Servo Motor (SG90)        | Rotates ultrasonic sensor for scanning area |
| Power Supply              | 9V battery or 2-cell LiPo                   |
| Jumper Wires / Chassis    | Standard car frame and wiring               |

# How It Works
1- The servo motor sweeps the ultrasonic sensor from side to side.

2- The sensor checks for obstacles in front, left, and right directions.

3- Based on the distance, the Arduino:

-Moves forward if the path is clear.

-Turns left or right if an obstacle is ahead.

-Stops if no clear path is found.

# Code Overview

- Libraries Used:

- AFMotor.h: Used to control the 4 DC motors via the L293D motor driver shield (Adafruit Motor Shield).

- Servo.h: Controls the servo motor that rotates the ultrasonic sensor.

- stdlib.h: Provides random() functionality to make movement decisions less predictable when obstacles are detected on both sides.

# Demo

https://github.com/user-attachments/assets/9aca30fd-a5c3-4031-9ad8-2160a31b3741

