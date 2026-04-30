# Skin Lesion Classification (Benign vs Malignant)

## Student Information

**Name:** Diane Lenhoff  
**Course:** ITAI 1378 – Computer Vision and AI  
**Project Type:** Tier 1 – Image Classification  
**Final Project Submission**

---

## Project Overview

This project uses computer vision and deep learning to classify skin lesion images as either **benign** or **malignant** using transfer learning with a pretrained ResNet18 model.

The goal is to support early screening by helping identify potentially dangerous skin lesions faster and more efficiently.

This project is for educational purposes only and is not intended to be used as a medical diagnostic tool.

---

## Problem Statement

Skin cancer can be difficult to detect early, and delayed diagnosis can lead to serious health risks.

Doctors, dermatologists, and patients benefit from faster screening tools that can help identify suspicious lesions earlier.

This project applies image classification to improve early detection support using deep learning.

---

## Solution Overview

The system takes an image of a skin lesion and:

1. Preprocesses the image
2. Uses a pretrained ResNet18 model
3. Predicts whether the lesion is benign or malignant
4. Provides confidence scores for predictions

---

## Technical Approach

### Computer Vision Technique

Image Classification

### Model Used

ResNet18 with Transfer Learning

### Frameworks

- Python
- PyTorch
- Torchvision
- Google Colab
- Matplotlib
- Scikit-learn

### Why This Approach

Transfer learning allows strong performance using smaller datasets and faster training times compared to training from scratch.

ResNet18 is efficient, accurate, and works well for image classification tasks.

---

## Dataset Plan

### Dataset Source

Public Kaggle Dataset: Skin Cancer – Malignant vs Benign

### Dataset Size

- Training Images: 2,637
- Testing Images: 660

### Labels

- Benign
- Malignant

### Preprocessing

- Resize images to 224x224
- Normalize pixel values
- Random horizontal flip
- Random rotation
- Training/testing split

---

## Final Results

### Performance Metrics

### Final Test Accuracy

**90.15%**

### Additional Metrics

- Precision
- Recall
- F1-score
- Confusion Matrix
- Sample Prediction Confidence Scores

### Speed Goal

Less than 1 second per image prediction

---

## Challenges and Solutions

| Challenge | Solution |
|---|---|
| Initial low accuracy (69.24%) | Reduced learning rate and trained additional epochs |
| Class imbalance | Used image augmentation |
| Limited training time | Used transfer learning with pretrained ResNet18 |

---

## Resources Used

| Resource | Details |
|---|---|
| Compute | Google Colab (GPU) |
| Framework | PyTorch |
| Dataset | Kaggle |
| Cost | Free |

---

## Demo Video

Demo video link: *(Paste your YouTube or Google Drive demo link here)*

---

## Repository Structure

```text
Skin-Lesion-Classification/
├── README.md
├── requirements.txt
├── notebooks/
│   └── Skin_Lesion_Classification_Final.ipynb
├── results/
│   ├── training_accuracy.png
│   ├── confusion_matrix.png
│   ├── classification_report.png
│   └── sample_predictions.png
└── docs/
    ├── AI_usage_log.md
    └── presentation.pdf
