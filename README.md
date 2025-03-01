# HACKATHON---bitwars
Hackathon - Sign language Interpreter
SignLy - AI Sign Language Interpreter
SignLy is an AI-powered platform designed to bridge communication gaps for the deaf and mute community by enabling real-time sign language interpretation. This system converts hand gestures from Indian Sign Language (ISL) into text and supports speech-to-text conversion to aid in communication.

Table of Contents
Project Overview
Features
Technologies Used
System Flow
Installation
Modules
Usage
Contributing
License
Contact
Project Overview
SignLy aims to enhance communication between deaf or mute individuals and the hearing population. With over 70 million people worldwide using sign language, SignLy offers an intuitive and efficient solution by providing AI-powered sign language recognition and speech-to-text capabilities.

Features
Indian Sign Language (ISL) Recognition: Converts hand gestures from ISL into readable text.
Speech-to-Text Conversion: Real-time conversion of spoken language into text.
Image Gallery: A comprehensive gallery of ISL symbols and gestures for learning.
User-Friendly Interface: Easy-to-navigate interface for quick gesture recognition.
Real-Time Interaction: Enables communication in real-time via gestures or speech.
Technologies Used
Frontend: HTML, CSS, JavaScript
Backend & Machine Learning: Flask (Python framework), TensorFlow (Keras), NumPy, OpenCV
Deployment: Flask API
Other Tools: Mediapipe for hand gesture detection
System Flow
Here’s a flowchart that outlines how the Sign Language Recognition system works:

Start - The system begins.
Capture Image from Camera - A user captures a gesture using the camera.
Pre-process Image - The image is pre-processed (e.g., resized and normalized) for model input.
Send Image to Backend - The processed image is sent to the backend server.
Model Predicts Gesture - The model predicts the gesture based on the image.
Display Prediction Result - The predicted result (text) is shown to the user.
Speech-to-Text Recognition - If there is speech input, it is converted into text for further interaction.
End - The process ends.
Installation
Follow these steps to set up SignLy locally:

Prerequisites
Python 3.8 or higher
Flask
TensorFlow
OpenCV
NumPy
Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/signly.git
cd signly
Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
Set Up Environment
Make sure to set up the environment variables as needed (e.g., Flask configuration).

Running the Application
Start the Flask server:

bash
Copy
Edit
python app.py
Now, you can access the application at http://localhost:5000.

Modules
1. Image Gallery
The Image Gallery is a resource to learn Indian Sign Language (ISL). It provides detailed images of gestures for various words and expressions. The gallery makes it easier for users to browse through signs and expand their vocabulary.

2. Mediapipe Landmark System
Mediapipe is used to detect hand landmarks from the image frame. By extracting these points, the system can interpret the gestures effectively, even in varying background and lighting conditions. OpenCV is used to draw the landmark points on a plain white background for better clarity.

3. Speech-to-Text Module
This module converts spoken language into text in real-time. It ensures seamless interaction between deaf/mute individuals and others, allowing communication through spoken language without any delays.

Usage
Once the platform is set up:

Capture Gesture: Point your camera at a sign language gesture and the system will interpret it into text.
Speech Recognition: Speak into the microphone, and the speech-to-text system will convert your speech into text for display.
Browse ISL Symbols: Use the ISL Image Gallery to learn signs and gestures.
