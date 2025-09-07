# Line_Follower_Robot


📌 Project: Arduino PID Line Follower Robot

📝 Description



This project presents an Arduino-powered PID Line Follower Robot that uses IR sensors to detect a path and PID control to navigate smoothly. The robot dynamically adjusts motor speeds to follow straight lines, curves, and sharp turns while minimizing oscillations. It can also handle U-turns, left/right turns, and dead ends with LED indicators.



⚡ Features

PID algorithm for smooth and stable navigation

4 IR sensors for line detection

Motor speed controlled with PWM signals

Handles sharp turns and U-turns

LED indicators for dead-end detection



🛠 Components Used

Arduino UNO / Nano

4 × IR Sensors

L298N Motor Driver

2 × DC Motors + Wheels

Robot Chassis

Power Supply (7.4V–12V battery)

2 × LEDs for indicators


📊 Working Principle

IR sensors detect the line and send signals to Arduino.

Arduino calculates an error value based on sensor readings.

The PID algorithm computes corrections:

PID=(Kp​×P)+(Ki​×I)+(Kd​×D)

Left and right motor speeds are adjusted accordingly:

Left speed = initial_speed - PID_value

Right speed = initial_speed + PID_value

The robot stays aligned with the line and makes smooth turns.



🔧 Circuit Connections

IR Sensors → Arduino Pins 2–5

Motor Driver (ENA/ENB, IN1–IN4) → Arduino Pins 6–11

LEDs → A3, A4

Motors → L298N Motor Driver

Power → 7.4V–12V Battery


▶️ How to Run

Connect the circuit as per the diagram.

Upload the provided Arduino code (line_follower.ino).

Place the robot on a track (black line on white surface).

Adjust Kp, Ki, Kd values if necessary for better performance.

Power the bot and watch it follow the line 🚗⚡.
