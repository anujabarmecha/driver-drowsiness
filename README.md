# driver-drowsiness
 Driver Drowsiness Detection Using CNN and Real-Time Video Monitoring
🚀 Overview
A real-time system that monitors driver drowsiness by analyzing eye and mouth states using a Convolutional Neural Network (CNN). The system detects closed eyes or yawning from webcam input and triggers audio-visual alerts to prevent fatigue-related accidents.

🎯 Features
Live face, eye, and mouth detection using OpenCV Haar cascades

Trained CNN model classifies eye states: open, closed, yawning

Real-time drowsiness alert using sound and text overlay

Image augmentation and dropout applied to prevent overfitting

🧠 Model Architecture
3 Convolutional layers with ReLU + MaxPooling

Dense layer with Dropout for regularization

Output layer with softmax activation for 4-class classification

Trained using Keras on custom eye/mouth dataset

🛠️ Tech Stack
Python, TensorFlow/Keras, OpenCV, Haar Cascades, ImageDataGenerator, NumPy / Pandas


🧪 How to Run
Clone the repository:


git clone https://github.com/your-username/driver-drowsiness-detection.git
cd driver-drowsiness-detection
Install dependencies:


pip install -r requirements.txt
Run real-time drowsiness detection:


python inference.py
🔔 Alert Logic
Eyes closed or yawning detected over multiple consecutive frames

Trigger:
Text warning on video feed
Audible beep alert (short-beep-tone.mp3)
