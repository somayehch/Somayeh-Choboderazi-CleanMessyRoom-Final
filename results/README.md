# Results Folder

This folder contains all the important images that show how my Clean vs. Messy Room classification model performed.  
Each picture gives visual proof of the model’s behavior, accuracy, and understanding of the data.

Below is an explanation of every image in this folder.

---

## 🖼️ sample_dataset.png — Preview of the Dataset
This picture shows a small sample of the images used to train and test the model.  
It helps confirm that the dataset loaded correctly and contains a variety of clean and messy rooms.

By looking at this preview, we can see:
- The dataset has both Clean and Messy examples  
- Images include different angles, lighting, and room sizes  
- Data quality is good enough for training a neural network  

This step is important because a model can only learn well if the dataset is correct.

---

## 📉 confusion_matrix.png — Model Performance Summary
This image shows the confusion matrix, which is one of the most important ways to evaluate a classification model.

The confusion matrix explains:
- How many Clean rooms were predicted correctly  
- How many Messy rooms were predicted correctly  
- Where the model made mistakes  
- Whether the model confuses one category with the other  

Correct predictions appear on the diagonal line.  
Mistakes appear in the other boxes.  
This gives a deeper understanding of the model's accuracy than just a single score.

---

## 🖼️ example_predictions_1.png — Example Model Predictions (Set 1)
This picture shows how the model predicts Clean and Messy rooms on real test images.

Each image includes the predicted label and whether it is correct.  
This helps us understand what the model is noticing, such as:

- Amount of clutter  
- Furniture organization  
- Visible floor space  
- Lighting and angle of the room  

Seeing prediction samples makes the model behavior easier to understand.

---

## 🖼️ example_predictions_2.png — Example Model Predictions (Set 2)
This is another set of prediction results, showing additional examples from the test dataset.

Different examples help show:
- Whether the model generalizes well  
- How it handles different room styles  
- How it responds to different levels of messiness  
- Whether the model is consistent in predicting clean vs messy rooms  

Multiple prediction sets provide a fuller picture of how the model performs overall.

---

## ✅ Summary
These images together help explain the whole project:

- **Dataset preview** shows the input the model learns from  
- **Confusion matrix** shows how accurate the model is  
- **Prediction examples** show real, visual results  

They make the project easier to understand and prove that the model works.
