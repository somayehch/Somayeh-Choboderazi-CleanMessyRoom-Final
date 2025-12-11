# Clean vs Messy Room Classifier – Final Project (ITAI-1378)- "Applied AI Portfolio - Houston Community College"

A Computer Vision system that predicts whether a room is Clean or Messy using a fine-tuned **ResNet50** deep learning model.
This project demonstrates skills in dataset creation, PyTorch training, transfer learning, evaluation, and creating a user-friendly demo interface.

---

## 👩‍💻 Author  
**Name:** Somayeh Choboderazi  
**Program:** Applied AI & Robotics – Houston Community College  
**Course:** ITAI 1378 – Computer Vision (Final Project)

---

## 📌 Project Overview

This project classifies room images into:

- **Clean Room**
- **Messy Room**

It includes the full AI development workflow:

- Creating a custom dataset  
- Preprocessing and organizing image data  
- Transfer learning with ResNet50  
- Training and validating the model  
- Evaluating performance  
- Building a simple user interface for real-world testing  

---

## 🧠 Model & Approach

**Framework:** PyTorch  
**Base Model:** ResNet50 (torchvision)  
**Method:** Transfer Learning  

### Steps:
1. Loaded a pretrained ResNet50  
2. Replaced the final layer for 2 classes  
3. Fine-tuned on custom dataset  
4. Saved final model as `model_final.pth`  

This method achieves strong performance even on smaller datasets.

---

## 🗂 Dataset

**Type:** Custom dataset using real room images**  

Collected using Bing Image Downloader with search terms:

- “clean bedroom real home”
- “messy bedroom real home”
- “clean living room real home”
- “messy kitchen real home”

Processed images were:

- cleaned manually


  
---

## 📈 Results

The model achieved strong generalization performance, including:

- **≈ 85–90% validation accuracy**  
- Sample predictions stored in `/results`  
- Evaluation results and screenshots included  

---

## 📘 Notebooks Overview

All project notebooks are organized in `/notebooks`:

1. **01_dataset_preparation.ipynb** – dataset creation  
2. **02_training.ipynb** – model training  
3. **03_evaluation.ipynb** – evaluation and testing  
4. **04_demo_user_interface.ipynb** – user-friendly image classifier demo  

Each notebook includes detailed markdown explanations and outputs.

---

## 🧩 Project Structure


- resized (224×224)  
- normalized  
- organized into:

----






- **GitHub:** https://github.com/somayehch

