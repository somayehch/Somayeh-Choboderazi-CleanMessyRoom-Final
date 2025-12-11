# Somayeh-Choboderazi-CleanMessyRoom-Final
# Clean vs Messy Room Classifier – Final Project (ITAI-1378)

A Computer Vision system that predicts whether a room is **Clean** or **Messy** using a fine-tuned **ResNet50** deep learning model.  
This project demonstrates practical skills in dataset creation, PyTorch training, transfer learning, evaluation, and building a simple user interface for real-world image classification.

---

## Author

**Name:** Somayeh Choboderazi  
**Program:** Applied AI & Robotics – Houston Community College  
**Course:** ITAI 1378 – Computer Vision (Final Project)

---

## Project Overview

The goal of this project is to train a deep learning model that can automatically classify images of rooms into two categories:

- Clean
- Messy

This work covers the full AI workflow:

1. Collecting and building a custom dataset  
2. Preprocessing and organizing image data  
3. Using transfer learning with ResNet50 (PyTorch)  
4. Training and evaluating the model  
5. Building a simple demo interface to test images

---

## Model and Approach

**Framework:** PyTorch  
**Base Model:** ResNet50 (from `torchvision.models`)  
**Technique:** Transfer Learning

Steps:

- Loaded a pretrained ResNet50 model
- Replaced the final classification layer with a custom layer for 2 classes (clean, messy)
- Fine-tuned the top layers on the custom dataset
- Used images resized to 224×224 and normalized

This approach allows good performance with a relatively small dataset by reusing strong image features learned from ImageNet.

---

## Dataset

**Type:** Custom dataset of real home images

The dataset was created by:

- Using Bing Image Downloader
- Searching for terms such as:
  - "clean bedroom real home"
  - "messy bedroom real home"
  - "clean living room real home"
  - "messy kitchen real home"
- Manually cleaning and filtering images
- Resizing and standardizing images
- Organizing them into folders:

```text
data/
   clean/
   messy/

