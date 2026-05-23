# 🔥 Fire Recognition with Machine Learning

> Real-time fire detection system using YOLOv8 and computer vision — built as part of academic project exhibition at VIT Bhopal University.
> **Grade: A (Excellent)**

---

## 📌 Overview

Traditional fire detection systems (smoke sensors, flame detectors) suffer from false alarms, limited coverage, and poor accuracy in large spaces. This project addresses those limitations by building an ML-powered fire recognition system that detects fire through image and video input using computer vision.

The system was trained on **706 annotated fire images** sourced from Roboflow and achieves approximately **80% detection accuracy**, with accuracy improving linearly with additional training sessions.

---

## 🧠 How It Works

1. **Data Collection** — 706 fire/non-fire images collected and annotated using Roboflow
2. **Model Training** — YOLOv8 object detection model trained using Ultralytics framework
3. **Performance Evaluation** — Cross-validation using Precision, Recall, and mAP metrics
4. **Real-time Testing** — Model tested on live video/image feeds via webcam

---

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3.10+ |
| ML Framework | YOLOv8 (Ultralytics) |
| Computer Vision | OpenCV |
| Data Annotation | Roboflow |
| Visualization | Matplotlib, IPython |
| Environment | Google Colab |

---

## 📊 Model Performance

| Metric | Value |
|---|---|
| Dataset Size | 706 images |
| Detection Accuracy | ~80% (3 training sessions) |
| False Positive Rate | Reduced vs traditional sensors |
| Projected Accuracy | 97–98% (with more training) |

---

## 🚀 How to Run

```bash
# Install dependencies
pip install ultralytics roboflow opencv-python matplotlib

# Run detection on an image
from ultralytics import YOLO
model = YOLO('yolov8s.pt')
results = model('your_image.jpg')
results[0].show()
```

Full training notebook available on Google Colab:
👉 [Open in Colab](https://colab.research.google.com/drive/1Jb4KQVyDmteNHiBjprtAore_ZOtNU0Lf?usp=sharing)

---

## 📁 Dataset

- Source: [Roboflow — Continuous Fire Dataset](https://universe.roboflow.com/-jwzpw/continuous_fire)
- Size: 706 annotated images
- Labels: Fire / No Fire

---

## ⚠️ Limitations

- Dataset size is relatively small (706 images) — accuracy improves with more data
- Currently detects fire only, not smoke
- Tested on laptop/PC — not yet deployed on IoT/edge devices
- Requires further training sessions for production-level accuracy

---

## 👥 Team

| Name | Roll No |
|---|---|
| Himangan Ghosh | 22MIM10002 |
| **Aishik Banerjee** | **22MIM10003** |
| Swarnika Chaki | 22MIM10044 |
| Bhupendra Yadav | 22MIM10097 |

**Guide:** Dr. Sarvanan S., VIT Bhopal University
**Institution:** VIT Bhopal University — School of Computing Science, Engineering & AI
**Year:** 2024
