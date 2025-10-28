# Gesture-Based Communication System

## Overview
A prosthetic glove system designed using flex sensors and Raspberry Pi to interpret hand gestures for speech-impaired users.  
The system converts gestures into text and speech output while integrating with a real-time health dashboard and emergency alert portal.

---

## Features
- Gesture recognition using flex sensors and MPU6050 motion sensors  
- Real-time text-to-speech conversion for verbal communication  
- IoT dashboard for live monitoring (temperature, pulse rate, emergency triggers)  
- Emergency alert system integrated with cloud API  
- Achieved 92% gesture recognition accuracy through calibration and filtering techniques  

---

## Tech Stack

| Component | Technology |
|------------|-------------|
| Hardware | Raspberry Pi, Flex Sensors, MPU6050, Wi-Fi Module |
| Software | Python, Flask, HTML/CSS Dashboard |
| Libraries | OpenCV, NumPy, SpeechRecognition, pyttsx3 |
| Platform | ThingSpeak / Firebase (for data sync) |

---

## System Architecture

```mermaid
flowchart TD
    A[Flex Sensors + MPU6050] -->|Analog Signals| B[Raspberry Pi Controller]
    B -->|Processed Data| C[Signal Processing & Gesture Classification]
    C -->|Recognized Gesture| D[Speech/Text Output]
    B -->|IoT Updates| E[IoT Dashboard + Emergency Alert Portal]

