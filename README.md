# yolo-player-tracker

Player Re-Identification Across Multiple Camera Angles with YOLOv11
This project aims to ensure that each player retains a consistent identity across two video feeds (broadcast.mp4 and tacticam.mp4) recorded from different camera perspectives during the same sports event. It uses a custom-trained YOLOv11 model for player detection and matches players using color histogram-based appearance features.

📌 Features

⚽ Detects players in both videos using YOLOv11.

🔁 Matches players across views based on HSV color histograms.

🗂️ Assigns consistent player_ids between video feeds.

🧠 How It Works
Detection: Runs inference using YOLOv11 to get bounding boxes of players in each frame.
Feature Extraction: Crops each player and extracts HSV color histograms.
Matching: Compares every detected player in tacticam to all players in broadcast using histogram correlation.
