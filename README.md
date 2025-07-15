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

## Running the Project

Clone the repository and run the main script on your input video:

```bash
git clone https://github.com/yourusername/football-analysis.git
cd football-analysis

python src/main.py --video videos/input/sample_match.mp4
```

Ensure you have the trained YOLOv5 model weights placed in the `models/` directory.

---

## Trained Models

* YOLOv5 trained for detection of football players, referees, and ball
* Sample annotated match video is included

---
Sample Output
A screenshot or video demo showing player tracking, possession percentages, and calculated distances can be included in the videos/output/ directory.

![Uploading Football.png…]()


---

## Future Work

* Add multi-camera tracking and player re-identification.
* Generate heatmaps for player movement and team formations.
* Integrate a dashboard for live match analytics and visualization.

---
