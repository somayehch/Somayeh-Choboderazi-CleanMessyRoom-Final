# Model Information – Clean vs Messy Room Classifier

This folder contains the trained model (or instructions to recreate it) for the Clean vs Messy Room Classification Final Project.

---

## Model File

The trained model used in this project is a fine-tuned ResNet50.

After training, the model was saved using the following command:

    torch.save(model.state_dict(), "model_final.pth")

If the model file (model_final.pth) is not included in this folder because it was too large to upload, you can recreate it by running:

1. notebooks/01_dataset_preparation.ipynb
2. notebooks/02_training.ipynb

Running these notebooks will generate a new model_final.pth.

---

## How to Load the Model

Use the following code to load the model for testing or the demo interface:

    import torch
    import torchvision.models as models

    model = models.resnet50(pretrained=False)

    num_ftrs = model.fc.in_features
    model.fc = torch.nn.Linear(num_ftrs, 2)

    model.load_state_dict(torch.load("models/model_final.pth", map_location=torch.device("cpu")))

    model.eval()

---

## Folder Structure

    models/
        model_final.pth   (optional)
        README.md         (this file)

---

## Note

If the model file is missing, this is normal.  
Your training notebook will recreate it automatically.
