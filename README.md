<h1 align="center">😴 Driver Drowsiness Detection</h1>
<p align="center">
  Real-time driver drowsiness detection system using CNN & InceptionV3 deep learning model.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Keras-D00000?style=flat&logo=keras&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white"/>
</p>

---

## 📌 Overview

A real-time drowsiness detection system that monitors a driver's eyes through a webcam. Using a trained **InceptionV3 CNN model**, it detects whether the driver's eyes are open or closed. If the eyes remain closed long enough, a **score variable** increases and an **alarm is triggered** to alert the driver — stopping only when the score drops back down.

---

## ✨ How It Works

1. 📷 **Webcam** captures live video frames
2. 👁️ **Haar Cascade** extracts the eye region from each frame
3. 🧠 **InceptionV3 CNN model** classifies eyes as open or closed
4. 📈 A **score variable** increases when eyes are detected closed
5. 🚨 **Alarm triggers** when score exceeds threshold
6. ✅ Alarm stops automatically when the driver opens their eyes

---

## 🏆 Model Performance

| Metric | Value |
|---|---|
| **Test Accuracy** | 95.55% |
| **Test Loss** | 0.1247 |
| **Architecture** | InceptionV3 (Transfer Learning) |

---

## 🛠️ Tech Stack

| Tool | Usage |
|---|---|
| TensorFlow / Keras | Model training & inference |
| InceptionV3 | CNN architecture (Transfer Learning) |
| OpenCV + Haar Cascade | Eye detection from video frames |
| NumPy | Data processing |
| Pygame / Playsound | Alarm sound |

---

## 📁 Project Structure

```
├── main.py                  # Real-time detection script
├── data_preparation.py      # Dataset loading & preprocessing
├── model.py                 # Model architecture & training
├── haarcascade/             # Haar Cascade XML files for eye detection
├── alarm.wav                # Alarm sound file
└── README.md
```

---

## 📦 Dataset

Data obtained from the **Media Research Lab (MRL)**.
Available at: [http://mrl.cs.vsb.cz/eyedataset](http://mrl.cs.vsb.cz/eyedataset)

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install tensorflow keras opencv-python numpy pygame
```

### Run
```bash
python main.py
```

---

## 👨‍💻 Author

**Mohamed Berhaila**
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/mohamed-berhaila)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat&logo=vercel&logoColor=white)](https://berhaila.com)