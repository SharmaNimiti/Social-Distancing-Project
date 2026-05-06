# 🚶‍♂️ Social Distancing Detection System using YOLOv3

![Python](https://img.shields.io/badge/Python-3.8+-blue)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green)
![Deep Learning](https://img.shields.io/badge/YOLOv3-Object%20Detection-orange)
![GPU](https://img.shields.io/badge/CUDA-Enabled-red)
![Status](https://img.shields.io/badge/Status-Active-success)
![License](https://img.shields.io/badge/License-MIT-green)

A real-time **Social Distancing Monitoring System** built using **YOLOv3 (Object Detection)** and **OpenCV**.  
The system detects people from live video feed and identifies **social distancing violations** based on distance between individuals.

---

## 🌟 Project Overview

This project uses **YOLOv3 deep learning model** to detect humans in a video stream and calculates the distance between them.  
If the distance between two individuals is below a predefined threshold, it flags them as a **violation**.

---

## 🚀 Features

### 🧍 Person Detection
- Detects humans using YOLOv3
- Filters only **person class (COCO dataset)**

---

### 📏 Distance Calculation
- Computes distance between detected individuals
- Uses center points of bounding boxes

---

### 🚨 Violation Detection
- Highlights:
  - 🔴 Red box → Violation
  - 🟢 Green box → Safe distance
- Displays total violation count

---

### 🎥 Real-Time Monitoring
- Uses webcam for live detection
- Processes frames continuously

---

### 💾 Video Output
- Saves processed video as:
  ```text
  output.avi

## 🛠️ Tech Stack
-Programming Language: Python
-Computer Vision: OpenCV (cv2)
-Deep Learning: YOLOv3
-Hardware Acceleration: CUDA (GPU support)
-Libraries: NumPy, PIL

## ⚙️ How It Works
1. Capture video from webcam
2. Load YOLOv3 model (weights + config)
3. Detect objects in each frame
4. Filter only "person" detections
5. Calculate distance between each pair
6. If distance < threshold:
     → Mark as violation
7. Draw bounding boxes:
     Red = Violation
     Green = Safe
8. Display and save output video

