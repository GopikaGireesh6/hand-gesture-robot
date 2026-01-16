
HAND GESTURE CONTROLLED ROBOT
Using ESP32 + WiFi + OpenCV + MediaPipe

==================================================

PROJECT OVERVIEW
This project demonstrates a robot that can be controlled using hand gestures.
A laptop camera captures the hand movements. OpenCV and MediaPipe process the video,
detect the hand landmarks, and recognize gestures. The recognized gesture is sent
through WiFi to an ESP32, which controls the robot’s motors accordingly.

==================================================

FEATURES

Real-time hand gesture recognition

Accurate hand tracking using MediaPipe

Video processing with OpenCV

Wireless control using WiFi

Fast and responsive robot movement

==================================================

HARDWARE REQUIREMENTS

ESP32 Development Board

Motor Driver (L298N / L293D)

DC Motors with Robot Chassis

Battery Pack

Jumper Wires

==================================================

SOFTWARE REQUIREMENTS

Python

OpenCV

MediaPipe

Arduino IDE

Socket Programming

==================================================



WORKING PRINCIPLE

Laptop camera captures hand gestures.

OpenCV reads and processes video frames.

MediaPipe detects hand landmarks.

Gestures are classified.

Command is sent via WiFi.

ESP32 receives command.

Motors move based on command.

==================================================

GESTURE TO ACTION MAPPING

Open Palm -> Move Forward
Fist -> Stop
Index Finger Up -> Turn Right
Index + Middle Up -> Turn Left
Thumb Up -> Move Backward

==================================================

