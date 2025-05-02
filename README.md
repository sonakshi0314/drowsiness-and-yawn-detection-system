# Drowsiness and Yawn Detection System
A real-time computer vision system designed to detect driver drowsiness and yawning using deep learning. 
This project aims to enhance road safety by alerting the driver when signs of fatigue are detected.

## 🚗 Overview
Driver drowsiness is a major cause of road accidents. This system leverages facial landmark detection and deep learning to monitor eye closure (drowsiness) and mouth opening (yawning) to identify signs of fatigue in real time. 
Upon detection, the system triggers an alarm to alert the driver.

## 🧠 Features
- Real-time video stream processing
- Eye aspect ratio (EAR) based drowsiness detection
- Mouth aspect ratio (MAR) based yawn detection
- Alarm system for fatigue alerts
- Modular and extendable codebase

## 🛠️ Technologies Used
- Python 3.x
- OpenCV
- dlib (for facial landmarks)
- NumPy
- imutils
- TensorFlow / Keras 

## 📁 Project Structure
1. dataset/ # Images/videos for training (if applicable)
2. model/ # Trained models (optional)
3. utils/ # Utility functions (EAR, MAR calculations, etc.)
4. main.py # Entry point for real-time detection
5. alarm.wav # Sound file for alerts
6. requirements.txt # Python dependencies
7. README.md # Project documentation

📐 How It Works
1. Eye Aspect Ratio (EAR): Calculates the ratio between the vertical and horizontal eye landmarks. If EAR is below a certain threshold for a number of frames, drowsiness is detected.
2. Mouth Aspect Ratio (MAR): Measures mouth openness. A high MAR for several frames indicates a yawn.
3. Alert System: An audio alert is triggered if drowsiness or yawning is detected.

📊 Future Improvements
-Integration with vehicle systems (e.g., automatic speed control)
-More robust model using deep learning-based face/eye detection
-Support for low-light or infrared conditions
-Mobile or embedded device deployment
