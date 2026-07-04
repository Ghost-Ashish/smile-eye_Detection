# 😊 Real-Time Face, Eye, and Smile Detection using OpenCV

## 📌 Project Overview

This project is a **real-time computer vision application** built using **Python** and **OpenCV**. It uses your computer's webcam to detect:

* 👤 Human Face
* 👀 Eyes
* 😊 Smile

Whenever a face is detected, a **green rectangle** is drawn around it. If eyes are detected, the text **"Eye Detect"** is displayed. If a smile is detected, the text **"Smiling"** appears on the screen.

The project uses **Haar Cascade Classifiers**, which are pre-trained XML models provided by OpenCV for object detection.

---

#
---

# Technologies Used

* Python 3.x
* OpenCV (cv2)
* Haar Cascade XML Models

---

# Project Structure

```
FACE & OBJECT DETECTION/
│
├── face_detection.py
├── haarcascade_frontalface_default.xml
├── haarcascade_eye.xml
├── haarcascade_smile.xml
└── README.md
```

---

# Requirements

Install Python packages:

```bash
pip install opencv-python
```

Check installation:

```bash
python -c "import cv2; print(cv2.__version__)"
```

---

# Haar Cascade Files

Download or use the following Haar Cascade XML files:

* haarcascade_frontalface_default.xml
* haarcascade_eye.xml
* haarcascade_smile.xml

Place all three XML files inside your project folder.


Press

```
Q
```

to quit.

---

# Detection Flow

```
Start

↓

Open Webcam

↓

Capture Frame

↓

Flip Image

↓

Convert to Gray

↓

Detect Face

↓

Detect Eyes

↓

Detect Smile

↓

Draw Rectangles

↓

Display Output

↓

Press Q?

↓

Yes → Exit

No → Continue
```

---

# Output

The application displays:

* Green rectangle around the face
* Blue rectangles around the eyes
* "Eye Detect" text
* "Smiling" text when a smile is detected

Everything runs live from the webcam.

---

# Advantages

* Lightweight
* Fast
* Easy to understand
* Beginner-friendly
* No deep learning required
* Works in real time

---

# Limitations

* Haar Cascades are less accurate than modern deep learning models.
* Performance may decrease in poor lighting.
* Large head rotations can reduce detection accuracy.
* Multiple faces may affect detection speed.

---

# Future Improvements

* Face recognition
* Face mask detection
* Emotion detection
* Age prediction
* Gender prediction
* Attendance system
* Face unlock system
* Drowsiness detection
* Object detection with YOLO
* Deep learning-based face detection

---

# Troubleshooting

## Webcam not opening

Check camera permissions.

Try:

```python
cap = cv2.VideoCapture(1)
```

if another camera index is being used.

---

## XML file not found

Verify the XML file paths.

Example:

```python
haarcascade_frontalface_default.xml
```

must exist at the specified location.

---

## No face detected

* Improve lighting.
* Face the camera directly.
* Keep a reasonable distance from the webcam.

---

# Learning Outcomes

After completing this project, you will understand:

* OpenCV basics
* Image processing
* Webcam handling
* Haar Cascade classifiers
* Face detection
* Eye detection
* Smile detection
* Region of Interest (ROI)
* Drawing shapes and text on images
* Real-time computer vision

---
