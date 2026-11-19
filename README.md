# Line Following Robot (LFR) 

An Arduino-based Line Following Robot designed to autonomously follow a track using a 14-channel sensor array and PD (Proportional-Derivative) control.

## Project Overview

This project explores autonomous robot navigation, sensor calibration, and motor speed control. The robot detects line positions using IR sensors and adjusts its motor speeds to stay on track.

## Key Features

- **14-Channel Sensor Array** — Detects line position and track changes.
- **PD Control Algorithm** — Adjusts motor speeds using proportional and derivative corrections.
- **Sensor Calibration** — Calibrates sensor readings for accurate line detection.
- **OLED Display Interface** — Provides menu-based configuration and sensor monitoring.
- **Adjustable Parameters** — Supports speed, Kp, Kd, and U-turn timing adjustments.
- **EEPROM Storage** — Saves calibration values and configuration settings.
- **Bluetooth Control Mode** — Supports serial commands for manual movement.
- **Motor Testing** — Includes built-in motor testing and configuration.

## Technologies and Components

- Arduino / Embedded C++
- IR Line Sensor Array
- LFR Carrier Board v1.3
- DC Motors and Motor Driver
- OLED Display (SSD1306)
- U8glib Library
- Arduino EEPROM Library

## How It Works

1. The sensor array reads the surface underneath the robot.
2. The program determines the line position from sensor readings.
3. The PD controller calculates the required correction.
4. Motor speeds are adjusted to keep the robot aligned with the track.
5. The robot performs recovery maneuvers when the line is lost.

## Getting Started

1. Install the Arduino IDE.
2. Install the U8glib library.
3. Open `LFR-Carrier-Board-v1.3-Demo-Code-1.ino`.
4. Select the appropriate board and port.
5. Upload the sketch to compatible hardware.
6. Calibrate the sensors and adjust the control parameters before operating.

## Project Status

Arduino firmware and configuration features are included. Hardware-specific tuning and performance verification depend on the robot setup.

## Acknowledgment

This repository uses the LFR Carrier Board v1.3 demo firmware as its starting point. Original demo-code credit belongs to its respective author or provider. Any personal modifications should be documented separately.
