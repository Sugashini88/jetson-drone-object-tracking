# jetson-drone-object-tracking
Real-time object detection and tracking on a drone gimbal using NVIDIA Jetson Orin, DeepStream, and YOLO.
# Jetson Drone Object Tracking

This project demonstrates **real-time object detection and tracking** on a **drone gimbal** using **NVIDIA Jetson Orin**, **YOLOv7**, and **DeepStream SDK**.  
It is designed for AI edge deployment where latency, power efficiency, and accuracy are critical.

---

## Overview

- **Platform:** NVIDIA Jetson Orin  
- **Frameworks:** DeepStream SDK, PyTorch  
- **Model:** YOLOv7 (custom-trained on drone-based dataset)  
- **Annotation Tool:** LabelMe  
- **Goal:** Detect and track moving targets from an onboard gimbal camera feed in real time.

---

##  Key Features

 Real-time object detection using YOLOv7  
 Multi-object tracking optimized for Jetson edge inference  
 Integration with drone gimbal camera  
 Dataset creation using LabelMe annotations  
 Visualization of performance metrics and training curves  

---

##  Project Structure

##  Training Details

- Model trained on a **custom drone dataset** annotated with LabelMe  
- Optimized for **low-latency edge inference**  
- Evaluation metrics visualized using YOLOv7’s built-in tools  

### Sample Training Results:
| Metric | Description |
|--------|--------------|
| Precision | Visualized in `PR_curve.png` |
| Confusion Matrix | Shown in `confusion_matrix.png` |
| Results Summary | Overall accuracy and F1 metrics (`results.png`) |

---

##  Demo Videos

Detection results on drone video feeds are available in the [`demo/`](demo/) folder:

- `demo1.mp4` – Object detection in aerial view  
- `demo2.mp4` – Tracking moving vehicles  
- `demo3.mp4` – Person tracking via gimbal  

---

## How to Run on Jetson Orin

1. **Flash Jetson Orin** with JetPack =6.1)
2. **Install NVIDIA DeepStream:**
   ```bash
   sudo apt update
   sudo apt install deepstream-7.1
