# 🦴 Bone Fracture Detection from X-rays Using Transfer Learning

This project focuses on developing a deep learning-based pipeline for detecting bone fractures from X-ray images using transfer learning. It demonstrates how computer vision and AI can support radiologists in early and accurate fracture diagnosis.

---

## 📁 Dataset

Collected and combined over 40,000 X-ray images from **eight public datasets**, including:

- GRAZPEDWRI-DX
- MURA
- MedPix
- Radiopaedia
- Orthopedic Image Database
- Others

### Labels:
- `0`: No Fracture  
- `1`: Fracture

---

## 🧪 Preprocessing

- Converted DICOM/PNG images to uniform format
- Resized images to 224x224 resolution
- Normalized pixel values
- Applied data augmentation: flipping, rotation, contrast variation
- Balanced classes through oversampling

---

## 🧠 Models

Used transfer learning with three architectures:

1. **ResNet-50**  
2. **EfficientNet-B0**  
3. **MONAI DenseNet-121**

Trained using PyTorch and MONAI with cross-entropy loss.

---

## 📊 Evaluation Metrics

- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**
- **Confusion Matrix**
- **ROC-AUC**

EfficientNet-B0 achieved the best performance (~98.9% test accuracy).

---

## ▶️ Usage

```bash
# Install dependencies
pip install torch torchvision monai opencv-python

# Run training
python train.py
```

---

## 📂 Folder Structure

```
bone_fracture_detection/
├── data/
│   └── train, test, valid sets
├── models/
│   └── best_model.pt
├── outputs/
│   └── metrics, plots, logs
├── src/
│   ├── dataset.py
│   └── train.py
└── README.md
```

---

## 📌 Key Highlights

- Trained on diverse fracture types and body parts
- Robust model performance with real-world deployment potential
- Designed for clinical aid in emergency and orthopedic radiology

---

## 👨‍💻 Author

Deniz Arda YILDIZ  
Email: [your.email@example.com]  
GitHub: [github.com/your-username]  
LinkedIn: [linkedin.com/in/your-profile]

---

## 📝 License

This project is open-source and available under the MIT License.
