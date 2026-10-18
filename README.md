# Smart Dustbin

Mini Project | B.Tech 3rd Year

A smart dustbin that automatically detects the presence of waste and classifies it as wet or dry using a soil moisture sensor. Based on the reading, the servo motor opens the lid to allow proper disposal.

## Project Overview

This project is designed to make waste segregation smarter and more efficient. It uses:
- an ultrasonic sensor to detect nearby objects,
- a soil moisture sensor to estimate whether the waste is wet or dry,
- a servo motor to open/close the bin lid automatically,
- an Arduino board to control the system.

## Features

- Automatic lid opening using a servo motor
- Waste detection using ultrasonic sensor
- Wet/dry classification using moisture sensing
- Real-time Serial Monitor output
- Simple and low-cost hardware design

## Components Used

- Arduino Uno
- Ultrasonic Sensor (HC-SR04)
- Soil Moisture Sensor
- Servo Motor
- Breadboard
- Jumper Wires
- Power Supply

## Circuit Connections

The project uses the following pin configuration in the code:

- Trig Pin: D12
- Echo Pin: D11
- Servo Signal Pin: D8
- Soil Sensor Pin: A0

You can also view the circuit diagram included in this repository:
- `circuit Diagram.png`

## Working Principle

1. The ultrasonic sensor measures the distance of an object in front of the bin.
2. If the object is within the set threshold distance, the system proceeds.
3. The soil moisture sensor reads the moisture level.
4. The system classifies the waste:
   - Wet waste if moisture is above the threshold
   - Dry waste otherwise
5. The servo motor rotates to open the lid accordingly.
6. The system resets after a short delay.

## Arduino Code

The project code is available in:
- `Source Code`

## Setup Instructions

1. Open the Arduino IDE.
2. Connect the hardware as per the circuit diagram.
3. Upload the code to the Arduino board.
4. Open the Serial Monitor.
5. Set the baud rate to `9600`.
6. Place an object near the sensor and observe the output.

## Example Serial Output

```text
Humidity: 71% Distance: 8 cm
==>WET Waste
