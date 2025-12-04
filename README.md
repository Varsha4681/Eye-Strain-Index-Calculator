# **📘 Overview**

This project implements a real-time eye strain monitoring system using Arduino Uno and OpenCV. The system measures three key parameters known to influence Digital Eye Strain (DES):

Ambient Light Intensity (lux)
Viewing Distance (cm)
Blink Rate (blinks/min)

An IR sensor detects user presence and activates the monitoring system. Data from hardware sensors are processed alongside computer-vision-based blink detection to compute a unified Eye Strain Index (ESI) indicating the user’s visual fatigue level.

## **🎯 Features**

Real-time measurement of lighting and viewing distance
Blink detection using OpenCV (EAR-based method)
Serial communication between Arduino and Python
Face-triggered activation using IR sensor
Eye Strain Index (ESI) calculation based on ergonomic thresholds
Suitable for personal wellness, ergonomic studies, and educational use

## **🛠 Technologies Used**
Arduino Uno
BH1750 Light Sensor
HC-SR04 Ultrasonic Sensor
E18-D80NK IR Sensor
Python, OpenCV, Mediapipe
Serial Communication (UART)

## **📐 Eye Strain Index (ESI)**

The ESI is computed using a weighted model based on ergonomic safety thresholds:

ESI = (Distance < 30 cm)*30 + (Lux < 200 lx)*30 + (Blink Rate < 15/min)*40

Higher ESI values indicate greater eye strain.

## **📄 Documentation**

The full project report—containing methodology, code, circuit design, and analysis—is provided in the repository.
