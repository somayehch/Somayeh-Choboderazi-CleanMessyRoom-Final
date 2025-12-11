# Model Information – Clean vs Messy Room Classifier

This folder contains the trained model (or instructions to recreate it) for the Clean vs Messy Room Classification Final Project.


## Model File

The trained model used in this project is a fine-tuned ResNet50.

After training, the model was saved using this command:

    torch.save(model.state_dict(), "model_final.pth")

If the model file (model_final.pth) is missing because it was too large to upload to GitHub, you can recreate it by running:

    notebooks/01_dataset_preparation.ipynb
    notebooks/02_training.ipynb

These notebooks will generate a new model_final.pth file.


## How to Load the Model

Use this code to load the trained model:

    import torch
    import torchvision.models as models

    model = models.resnet50(pretrained=False)

    num_ftrs = model.fc.in_features
    model.fc = torch.nn.Linear(num_ftrs, 2)

    model.load_state_dict(torch.load("models/model_final.pth", map_location=torch.device("cpu")))

    model.eval()



