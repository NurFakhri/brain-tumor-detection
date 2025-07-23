# Brain Tumor Detection on MRI Images 🧠🩻

This project aims to build an image classification model to detect brain tumors using MRI scans. The goal is to classify MRI images into four categories: **No Tumor**, **Pituitary**, **Meningioma**, and **Glioma**.

## 📁 Dataset
We used a publicly available MRI brain tumor dataset containing four classes:
- `no_tumor/`
- `pituitary/`
- `meningioma/`
- `glioma/`

Each image was resized to `224x224` and normalized before training.

## ⚙️ Model
- **Architecture**: ResNet50 (Transfer Learning)
- **Epochs per experiment**: 25
- **Preprocessing methods used**: CLAHE, Gaussian Blur (to observe effects)
- **Grad-CAM**: For model interpretability and tumor region focus

## 📊 Key Insights
- CLAHE preprocessing improved classification performance by enhancing local contrast.
- Gaussian blur reduced performance due to loss of critical tumor edge details.
- Some Grad-CAM results showed focus on irrelevant regions, suggesting room for model refinement.
- Clinical expert validation is recommended before deployment.

