✋ Real-Time Hand Detection Using MediaPipe & OpenCV

This project implements real-time hand detection and landmark visualization using MediaPipe and OpenCV.
It detects a hand from the webcam feed and draws custom “pipe-like” connections between hand landmarks to visually represent finger and wrist structure.

🚀 Features

Real-time webcam hand detection

MediaPipe Hand Landmarker Task API

Custom hand landmark connections (pipes)

Smooth visualization using OpenCV

Lightweight and beginner-friendly computer vision project

⚠️ Important Setup Note (First Hurdle)

MediaPipe currently does NOT fully support Python 3.11+.

🔹 This project requires:

Python 3.8 – 3.10


Setting up the correct Python version and environment was the first major challenge of this project and an important learning experience.

📂 Project Structure
├── hand_detection.py          # Main Python script
├── hand_landmarker.task       # MediaPipe hand model file
└── README.md                  # Project documentation

🛠️ Installation & Setup
1️⃣ Create a Virtual Environment (Recommended)
python -m venv venv
source venv/bin/activate        # Linux / Mac
venv\Scripts\activate           # Windows

2️⃣ Install Dependencies
pip install opencv-python mediapipe

3️⃣ Download MediaPipe Model

Download the Hand Landmarker model from MediaPipe and place it in the project directory:

hand_landmarker.task

▶️ How to Run
python hand_detection.py


Press ESC to exit the application.

Make sure your webcam is connected.

🧠 How It Works

Captures video frames using OpenCV

Converts frames to RGB format

Uses MediaPipe Hand Landmarker to detect hand landmarks

Maps normalized landmark coordinates to pixel values

Draws:

Lines between connected landmarks (pipes)

Circles at each landmark point

📸 Sample Output

Hand detected in real time

Green lines show finger & wrist connections

Red circles represent individual landmarks

(Add screenshots here for better visualization)

🧰 Tech Stack

Python

OpenCV

MediaPipe

Computer Vision

Git & GitHub

🌟 Key Learnings

MediaPipe Task-based API usage

Real-time computer vision processing

Landmark coordinate mapping

Dependency & environment management

Python version compatibility issues

🚀 Future Improvements

Gesture recognition (pinch, swipe, count fingers)

Hand-controlled volume or brightness

Two-hand detection

Integration with Machine Learning models

🤝 Contributing

Contributions are welcome!
Fork the repository, improve features, and submit a pull request.

