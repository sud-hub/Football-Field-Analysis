# ⚽ Football Analysis Project

## 📌 Introduction

This project aims to detect and track **players**, **referees**, and the **football** from match footage using advanced computer vision techniques.

We leverage **YOLOv5** for object detection and further enhance the system by:

* Segmenting and clustering jersey colors to **assign players to teams**.
* Measuring **ball acquisition percentage** per team.
* Using **optical flow** for camera movement estimation.
* Applying **perspective transformation** to measure **player speed and distance in meters**.

The goal is to analyze player movements and performance — making this an ideal project for real-world CV applications in sports analytics.

---

## 🎯 Key Features

* ✅ **Object Detection**: Detect players, ball, referees using **YOLOv5**
* 🎽 **Team Identification**: Use **KMeans clustering** on jersey colors
* ⚽ **Ball Possession Metrics**: Calculate team-wise ball acquisition percentage
* 🎥 **Optical Flow**: Estimate camera movement for accurate player tracking
* 🧭 **Perspective Transformation**: Convert pixel movement to real-world meters
* 🏃 **Player Stats**: Compute **distance covered** and **speed**

---

## 🧠 Techniques & Modules Used

| Module                    | Purpose                                              |
| ------------------------- | ---------------------------------------------------- |
| **YOLOv5 (Ultralytics)**  | Real-time object detection (players, ball, referees) |
| **KMeans Clustering**     | Group players by jersey color to identify teams      |
| **Optical Flow**          | Track frame-to-frame camera movement                 |
| **Perspective Transform** | Map pixel movement to real-world scale               |
| **OpenCV + NumPy**        | Image/video processing, mathematical operations      |
| **Matplotlib, Pandas**    | Visualization and data handling                      |

---

## 🏋️ Trained Models

* ✅ YOLOv5 trained for player, referee, and ball detection
* Sample annotated input video included

---

## 🛠️ Requirements

Install the following libraries to run the project:

```bash
pip install ultralytics opencv-python numpy matplotlib pandas supervision
```

---

## ▶️ Run the Project

```bash
# Step 1: Clone the repository
git clone https://github.com/yourusername/football-analysis.git
cd football-analysis

# Step 2: Run the main script
python src/main.py --video videos/input/match_sample.mp4
```

---

## 📸 Screenshot

![Demo Output](assets/demo_screenshot.png)

---

## 📈 Future Enhancements

* Add player re-identification across multiple cameras
* Integrate heatmaps and possession charts
* Deploy as a web dashboard for live analytics

---
