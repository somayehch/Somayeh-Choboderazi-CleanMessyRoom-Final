# Dataset Information – Clean vs Messy Room Classification

This project uses a **custom dataset** of real home images collected for the purpose of training a deep learning model to classify rooms as **Clean** or **Messy**.

The full dataset is **not included** in this repository because:
- It contains images downloaded from online sources
- The total size is too large for GitHub
- Some images may not be licensed for redistribution

This README explains how the dataset was created and how you can recreate it if needed.

---

## 📁 Dataset Structure

The dataset was organized into two main folders:


- **clean/** contains images of neat, organized rooms  
- **messy/** contains images of cluttered or disorganized rooms  

All images were resized and cleaned before training.

---

## 🌐 How the Dataset Was Collected

Images were collected using **Bing Image Downloader**, using search queries such as:

- "clean bedroom real home"
- "messy bedroom real home"
- "clean living room real home"
- "messy kitchen real home"
- "clean office real home"
- "messy room realistic"

Steps taken during dataset creation:
1. Collected image batches for each keyword  
2. Removed duplicates and corrupted files  
3. Verified images were actual indoor rooms  
4. Resized images to **224 × 224**  
5. Saved them into `clean/` and `messy/` folders  

---

## 🔢 Dataset Size

Approximately **280 total images**, balanced between:

- Clean: ~140  
- Messy: ~140  

This size works well with **transfer learning** using ResNet50.

---

## 🧹 Preprocessing Steps

Before training, images were:

- Resized to 224×224  
- Normalized to match ImageNet mean/std  
- Augmented with random transforms (if used) such as:
  - Horizontal flip  
  - Rotation  
  - Color jitter  

These steps improved the model’s performance and generalization.

---

## 📝 Notes

If you'd like to recreate the dataset:
- Use the search keywords above  
- Collect images of real home environments  
- Avoid staged or unrealistic photos  
- Keep image dimensions consistent  
- Maintain a balanced number of clean and messy examples  

---

If this dataset is needed for grading or verification, please contact the project author directly.
