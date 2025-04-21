🚗 Driver Drowsiness Detection System
A real-time driver drowsiness detection system using Python, OpenCV, and dlib. This project helps prevent road accidents by alerting the driver when signs of fatigue or drowsiness are detected through eye movement monitoring.

🔍 Overview
Fatigue is a major factor in traffic accidents. This system uses a webcam to track the driver’s eye aspect ratio (EAR) and sets off an alarm if the eyes remain closed for too long, indicating the driver might be falling asleep.

🎯 Features
Real-time webcam-based detection

Eye aspect ratio (EAR) calculation

Facial landmark detection with dlib

Visual alert on screen + audible alarm using pygame

Simple and lightweight codebase

🛠️ Technologies Used
Python

OpenCV

dlib

imutils

scipy

pygame

📁 Project Structure
bash
Copy
Edit
Driver-Drowsiness-Detection/
│
├── shape_predictor_68_face_landmarks.dat  # Pretrained facial landmark model
├── music.wav                              # Alarm sound file
├── drowsiness_detection.py                # Main Python script
├── README.md                              # Project documentation
📦 Installation & Setup
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/driver-drowsiness-detection.git
cd driver-drowsiness-detection
Install required libraries:

bash
Copy
Edit
pip install opencv-python dlib imutils pygame scipy
Download the dlib model:

Download shape_predictor_68_face_landmarks.dat from:
http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2

Extract and place it in your project directory.

Run the script:

bash
Copy
Edit
python drowsiness_detection.py
⚙️ How It Works
Uses dlib to detect facial landmarks

Calculates the Eye Aspect Ratio (EAR) for both eyes

If EAR is below a threshold (e.g., 0.25) for a set number of frames, an alert is triggered

An alarm sound is played to wake the driver

📷 Sample Output
When drowsiness is detected, the screen displays:

markdown
Copy
Edit
****************ALERT!****************
And a sound alarm is played using music.wav.

📌 Notes
Ensure your webcam is connected and accessible

Place music.wav and the .dat model file in the same directory as the script

Works best in good lighting conditions

🤝 Contributing
Contributions, suggestions, and improvements are welcome!
Feel free to open issues or submit pull requests.

📄 License
This project is licensed under the MIT License.

🙌 Acknowledgements
dlib

OpenCV

Inspired by real-world vehicle safety applications

Made with ❤️ for safe and smart driving.