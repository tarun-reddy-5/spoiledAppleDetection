# Spoiled Apple Detector

The **Spoiled Apple Detector** is a machine learning project designed to identify spoiled apples in a batch of apples, aiming to reduce food wastage. By detecting and separating spoiled apples, this tool can help extend the shelf life of good apples and prevent further spoilage. The project leverages state-of-the-art computer vision techniques like **YOLO** for object detection and **MobileNetV2** for classification.

## Table of Contents
- [Introduction](#introduction)
- [Inspiration](#inspiration)
- [Usage](#usage)
- [Project Overview](#project-overview)

## Introduction
The **Spoiled Apple Detector** is designed to address food spoilage in apples, which is a significant contributor to food wastage globally. This solution can be extended to detect spoilage in other types of food, making it a valuable tool for reducing waste in various contexts.

## Inspiration
With food wastage being a global issue, I was inspired to find a solution that could help minimize this problem. By detecting spoiled apples early on, we can prevent the spoilage of other food items and help consumers make better use of their food supplies.

## Usage

1. **Upload Images**: Use the 'predictor.ipynb' notebook to upload images of apples.
2. **Detection & Classification**: The YOLO model detects apples, and the binary classifier determines if they are "Good" or "Spoiled."
3. **Results**: The system returns an image highlighting the spoiled apples in red boxes and good apples in green boxes.

## Project Overview
This project uses a combination of object detection and binary classification to identify spoiled apples within a batch. The system works as follows:
- **Data Collection**: Images of good and spoiled apples were collected.
- **Binary Classifier**: I fine-tuned the `MobileNetV2` model to create a binary classifier that distinguishes between good and spoiled apples.
- **YOLO Integration**: YOLO was fine-tuned to detect apples in images. The detected apples were passed to the classifier for final prediction.
- **Prediction Pipeline**: The system first detects apples using YOLO, then classifies each apple as either "Good" or "Spoiled" using the binary classifier.
