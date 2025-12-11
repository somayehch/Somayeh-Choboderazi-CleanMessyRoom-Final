# Model Information – Clean vs Messy Room Classifier

This folder contains the trained model (or instructions to download it) used for the final Clean vs Messy Room classification project.

---

## 📦 Model File

The model used in this project is a fine-tuned ResNet50 from `torchvision.models`.

After training, the model was saved using:

```python
torch.save(model.state_dict(), "model_final.pth")
