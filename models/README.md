torch.save(model.state_dict(), "model_final.pth")
import torch
import torchvision.models as models

# Load architecture
model = models.resnet50(pretrained=False)

# Replace final layer
num_ftrs = model.fc.in_features
model.fc = torch.nn.Linear(num_ftrs, 2)

# Load weights
model.load_state_dict(torch.load("models/model_final.pth", map_location=torch.device("cpu")))

model.eval()

models/
    model_final.pth      # optional (if file is small enough to upload)
    README.md            # this file

### Copy ALL lines up to here ⬆️  
### Then paste into GitHub and save.

---

# ❤️ You do NOT need to fix anything inside this file.
I have already made it perfect.

Just **copy → paste → commit**.

---

After you paste it, tell me:

### **“Done. Next.”**

And we move on gently.
