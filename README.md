# Traffic Analysis Using YOLOv8

## Overview
This project implements a real-time traffic analysis system using the YOLOv11 object detection model. It processes video frames to detect vehicles, evaluates traffic intensity, and logs the results. The system allows users to define an Area of Interest (AOI) for vehicle counting and provides metrics for performance evaluation.

## Features
- **Load Pre-trained Model**: Utilizes a YOLOv11 model (`yolo11n.pt`) for vehicle detection.
- **Traffic Intensity Classification**: Classifies traffic intensity into four categories:
  - No Traffic
  - Low Traffic
  - Medium Traffic
  - High Traffic
- **Area of Interest (AOI) Definition**: Users can define a polygonal AOI using mouse events to focus on specific areas in the video.
- **Real-time Processing**: Processes video frames in real-time, displaying detected vehicles and traffic intensity.
- **Ground Truth Logging**: Saves ground truth data for each frame in JSON format.
- **Excel Logging**: Saves traffic analysis data to an Excel file for further analysis.

## Requirements
- Python 3.7 or higher
- Required libraries:
  ```bash
  pip install opencv-python numpy ultralytics pandas scikit-learn
