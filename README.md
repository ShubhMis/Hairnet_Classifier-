# Hairnet_Classifier-
# Hairnet Classifier

A two-stage computer vision pipeline for detecting whether a person is wearing a hairnet, designed for food safety and industrial compliance scenarios.

## 📌 Overview
This project uses:
1. **YOLOv8** for person/head detection
2. **Vision Transformer (ViT)** classifier to determine:
   - `hairnet`
   - `no_hairnet`

The system is trained on a custom dataset cropped person images, labeled in YOLO format, and optimized for deployment in real-time monitoring systems.

## ✨ Features
- **Two-stage detection:**  
  First stage detects persons; second stage classifies cropped images.
- **Custom dataset training:**  
  YOLO format labels with classes `[hairnet, no_hairnet]`.
- **From-scratch ViT training:**  
  Uses cropped detections as input, without relying on pretrained weights.
- **Confidence scores** for each classification.
- **Evaluation metrics**: accuracy, confusion matrix, precision, recall, F1-score.

## 📂 Project Structure
