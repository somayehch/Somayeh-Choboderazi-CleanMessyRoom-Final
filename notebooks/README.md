# Notebooks Overview – Clean vs Messy Room Classifier

This folder contains all Jupyter notebooks used in the Clean vs Messy Room Final Project for ITAI-1378 (Computer Vision).

Each notebook represents a different stage of the AI workflow.

---

## 1. Dataset Preparation Notebook

**File:** 01_dataset_preparation.ipynb  
**Purpose:**  
- Downloads images for clean and messy rooms  
- Removes corrupted files  
- Resizes and normalizes images  
- Organizes data into folder structure  
- Splits into training and validation sets  

---

## 2. Model Training Notebook

**File:** 02_training.ipynb  
**Purpose:**  
- Loads the dataset  
- Applies data transformations  
- Uses transfer learning with ResNet50  
- Trains the classifier  
- Saves the trained model as `model_final.pth`  

---

## 3. Evaluation Notebook

**File:** 03_evaluation.ipynb  
**Purpose:**  
- Loads the trained model  
- Evaluates accuracy on validation data  
- Displays predictions  
- Shows example outputs  

---

## 4. Demo User Interface Notebook

**File:** 04_demo_user_interface.ipynb  
**Purpose:**  
- Provides a simple user interface to test images  
- Lets users upload an image and see prediction  
- Uses the saved model for inference  

---

## Notes

- Make sure all notebooks have been run before uploading  
- Output images and screenshots should be saved in `/results`  
- If the model file is missing, re-run the training notebook  
