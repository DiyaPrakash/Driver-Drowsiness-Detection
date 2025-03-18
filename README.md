# Drowsiness & Yawn Detection

## Overview
This project implements a **real-time drowsiness and yawn detection system** using **computer vision and deep learning**. It continuously monitors a user’s face through a webcam and alerts them when drowsiness or excessive yawning is detected.

## Features
- Detects **eye aspect ratio (EAR)** to identify drowsiness.
- Measures **lip distance** to detect yawning.
- Uses **Haar cascade and dlib’s facial landmark predictor** for face and feature detection.
- Issues an **alert sound** when drowsiness or yawning is detected.

## Technologies & Libraries Used
- **Computer Vision**: OpenCV, imutils  
- **Facial Landmark Detection**: dlib, Haar Cascade Classifier  
- **Deep Learning**: Scipy, NumPy  
- **Multithreading & Sound Alerts**: Threading, Playsound  

## Installation & Setup
### 1. Clone the Repository
```sh
git clone <repository-url>
cd <repository-folder>
```

### 2. Install Dependencies
```sh
pip install -r requirements.txt
```

### 3. Run the Detection System
```sh
python drowsiness_yawn.py --webcam 0
```

## Usage
- The system captures real-time video and detects drowsiness or yawning.
- If **eye aspect ratio (EAR) drops** below the threshold for a set duration, a **drowsiness alert** is triggered.
- If **lip distance exceeds** the yawn threshold, a **yawn alert** is triggered.
- The system **plays an alarm sound** to alert the user.

## License
This project is open-source and available under the **MIT License**.

