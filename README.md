PROJECT DESCRIPTION
This project controls a robot using hand gestures.
A laptop camera captures hand movements.
OpenCV and MediaPipe detect and classify the gesture.
The gesture command is sent through WiFi to an ESP32.
ESP32 receives the command and controls the motors.

FEATURES

Real-time hand gesture recognition

MediaPipe hand tracking

OpenCV video processing

WiFi communication

Low latency robot control

HARDWARE USED

ESP32 Development Board

Motor Driver (L298N / L293D)

DC Motors and Robot Chassis

Battery Pack

Jumper Wires

SOFTWARE USED

Python

OpenCV

MediaPipe

Arduino IDE

Socket Programming (WiFi)

PROJECT STRUCTURE

Hand-Gesture-Controlled-Robot
|
|-- esp32_code
| |-- robot_control.ino
|
|-- python_code
| |-- gesture_control.py
|
|-- requirements.txt
|-- README.txt

HOW IT WORKS

Laptop camera captures hand movement

OpenCV reads the video frames

MediaPipe detects hand landmarks

Gesture is identified

Command is sent via WiFi

ESP32 receives command

Motors move according to command

GESTURE MAPPING

Open Palm -> Forward
Fist -> Stop
Index Finger Up -> Right
Index + Middle -> Left
Thumb Up -> Backward

SETUP STEPS

Clone the repository
git clone https://github.com/your-username/hand-gesture-robot.git

Install Python libraries
pip install -r requirements.txt

Upload ESP32 Code

Open robot_control.ino

Select ESP32 board in Arduino IDE

Set WiFi SSID and Password

Upload the code

Run the Gesture Program
python python_code/gesture_control.py

DATA FLOW

Camera -> OpenCV -> MediaPipe -> WiFi -> ESP32 -> Motor Driver -> Robot

TESTING

Test gesture detection without robot first

Check WiFi connection

Verify motor wiring

Monitor serial output

FUTURE IMPROVEMENTS

Add more gestures

Obstacle detection

Mobile app control

Better gesture accuracy
