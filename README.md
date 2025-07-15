# Football Analysis Project

## Introduction

This project aims to detect and track players, referees, and the football from match footage using advanced computer vision techniques. The objective is to analyze player movement and team performance by leveraging object detection, clustering, and motion tracking methods.

The pipeline includes:

* Detecting players and objects using YOLOv5.
* Assigning players to teams using KMeans clustering on jersey colors.
* Calculating ball acquisition percentage per team.
* Estimating camera motion using optical flow.
* Applying perspective transformation to convert pixel-based tracking into real-world distance.
* Computing each player's speed and total distance covered during the match.

This project brings together multiple computer vision concepts to perform in-depth sports analysis on real-world football videos.

---

## Key Features

* Object detection using YOLOv5 for players, referees, and the football.
* Team assignment based on jersey color using KMeans clustering.
* Possession analysis based on team-wise ball control over time.
* Player movement analysis with optical flow and motion tracking.
* Perspective transformation for accurate measurement of real-world distances.
* Speed and distance metrics computed per player.

---

## Techniques and Libraries Used

| Technique / Library        | Description                                         |
| -------------------------- | --------------------------------------------------- |
| YOLOv5 (Ultralytics)       | Object detection for players, ball, referees        |
| OpenCV                     | Image and video processing                          |
| KMeans (from scikit-learn) | Clustering pixels to identify team jersey colors    |
| Optical Flow               | Camera motion estimation across video frames        |
| Perspective Transform      | Mapping frame coordinates to real-world coordinates |
| NumPy, Pandas, Matplotlib  | Data handling and visualizations                    |
| Supervision                | Object tracking and video annotation utilities      |

---

## Requirements

To run this project, the following libraries are required:

```bash
pip install ultralytics opencv-python numpy matplotlib pandas supervision
```

---

## Trained Models

* YOLOv5 trained for detection of football players, referees, and ball
* Sample annotated match video is included

---
Sample Output


<img width="2468" height="1276" alt="Football" src="https://github.com/user-attachments/assets/06027459-60a2-4ad5-9b6b-e5f818fb84d4" />
---

## Future Work

* Add multi-camera tracking and player re-identification.
* Generate heatmaps for player movement and team formations.
* Integrate a dashboard for live match analytics and visualization.

---
