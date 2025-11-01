# 🚗 Driver Alert System using Machine Learning & Deep Learning

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green.svg)
![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)

---

## 📖 Overview

**Driver Alert System** is an AI-powered real-time safety monitoring solution that detects **driver drowsiness, yawning, and inattention** using **Machine Learning (ML)** and **Deep Learning (DL)** techniques.  

The primary goal is to **enhance road safety** by providing timely alerts when a driver shows signs of fatigue or distraction.  
By leveraging **computer vision, facial landmark detection, and neural networks**, the system can monitor the driver’s facial behavior continuously through a webcam or in-car camera.

---

## 🚀 Features

- 🧠 **Real-time Drowsiness Detection** using Eye Aspect Ratio (EAR) and Mouth Aspect Ratio (MAR)  
- 👁️ **Facial Landmark Tracking** via OpenCV & Dlib/MediaPipe  
- 🔊 **Instant Alerts** (sound or visual cues) when fatigue is detected  
- 🧩 **Hybrid ML + DL Model** for improved detection accuracy  
- ⚙️ **Customizable thresholds** and temporal smoothing for robustness  
- 📈 **Performance metrics** such as accuracy, precision, recall, and F1-score  
- 🧠 **Deployable** on edge devices like Raspberry Pi or Jetson Nano  

---

## 🧩 System Architecture

1. **Video Capture:**  
   - Captures real-time video frames from the driver’s camera feed.
2. **Face & Landmark Detection:**  
   - Detects facial regions like eyes and mouth using Dlib/MediaPipe or Haar cascades.
3. **Feature Extraction:**  
   - Calculates Eye Aspect Ratio (EAR) and Mouth Aspect Ratio (MAR).
4. **Behavior Analysis:**  
   - Identifies prolonged eye closure or yawning using heuristic + ML/DL models.
5. **Alert Generation:**  
   - Triggers alarms or notifications if drowsiness is detected for consecutive frames.

---

## 🧠 Technologies Used

| Category | Tools / Frameworks |
|-----------|--------------------|
| **Programming Language** | Python 3.x |
| **Deep Learning Frameworks** | TensorFlow / Keras |
| **Machine Learning Libraries** | scikit-learn |
| **Computer Vision** | OpenCV, Dlib / MediaPipe |
| **Data Processing** | NumPy, Pandas |
| **Visualization** | Matplotlib, Seaborn |
| **Model Deployment (optional)** | Flask / Streamlit |

---

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/srihith07/Driver_alert_system.git
   cd Driver_alert_system
Create and activate a virtual environment

bash
Copy code
python -m venv venv
venv\Scripts\activate        # For Windows
source venv/bin/activate     # For macOS/Linux
Install dependencies

bash
Copy code
pip install -r requirements.txt
Run the script

bash
Copy code
python src/main.py
📂 Project Structure
bash
Copy code
Driver_alert_system/
│
├── dataset/
│   ├── train/
│   ├── test/
│   └── validation/
│
├── models/
│   └── driver_drowsiness_model.h5
│
├── src/
│   ├── main.py
│   ├── train.py
│   ├── utils/
│   │   ├── face_detector.py
│   │   ├── landmarks.py
│   │   ├── features.py
│   │   └── alert_system.py
│
├── assets/
│   ├── demo_drowsy.jpg
│   ├── demo_alert.jpg
│   └── demo.gif
│
├── requirements.txt
├── README.md
└── LICENSE
📊 Results
Metric	Score
Accuracy	97.3%
Precision	96.8%
Recall	95.9%
F1-Score	96.3%

(Results may vary depending on dataset size, thresholds, and lighting conditions.)

Example Output:

⚙️ Configuration Parameters
Parameter	Description	Default
EAR_THRESHOLD	Minimum EAR for detecting eye closure	0.20
EAR_CONSEC_FRAMES	Frames required for alert	48
MAR_THRESHOLD	Threshold for yawning detection	0.6
SMOOTH_WINDOW	Temporal smoothing window	10

All parameters are configurable via src/main.py.

🧪 Future Enhancements
🚘 Integration with vehicle telemetry (CAN bus) for smarter context-aware alerts

🌍 Multi-camera support for fleet monitoring

⚡ Edge optimization using TensorFlow Lite or ONNX

📱 Mobile app or dashboard interface for monitoring and reporting

🔋 Adaptive threshold tuning using Reinforcement Learning

🤝 Contributing
Contributions are welcome!
If you'd like to enhance the model, add features, or optimize performance, please fork the repo and submit a pull request.

Steps:

bash
Copy code
git fork https://github.com/srihith07/Driver_alert_system.git
git checkout -b feature-name
git commit -m "Added new feature"
git push origin feature-name
📜 License
This project is licensed under the MIT License — see the LICENSE file for details.

👨‍💻 Author
Srihith Netha
📧 srinetha001@gmail.com
💻 GitHub Profile
💼 LinkedIn

“Empowering safer roads through intelligent driver monitoring.”
