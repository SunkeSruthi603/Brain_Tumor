# Brain Tumor Detection using Deep Learning

A deep learning-based model to detect brain tumors from MRI images, trained and evaluated in Google Colab. This project leverages convolutional neural networks (CNNs) for image classification and aims to assist in the early diagnosis of brain tumors.

---

##Table of Contents

- [Demo](#-demo)
- [Features](#-features)
- [Dataset](#-dataset)
- [Model Architecture](#-model-architecture)
- [Training Details](#-training-details)
- [How to Use](#-how-to-use)
- [Results](#-results)
- [Future Work](#-future-work)
- [License](#-license)

---

##Demo

> ![image](https://github.com/user-attachments/assets/0fbd99a7-457b-4fc6-a4e1-e35875720234)
> [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1MRhLiGPGnYemvDd_WRTh6VWrW9tg1y1n#scrollTo=RDIRJOEI0MpZ)

---

##Features

- Classification of MRI brain scans as Tumor (Tumor Type) / No Tumor
- CNN-based image classifier
- Trained using data augmentation
- Built and trained on Google Colab

---

## Dataset

- Dataset Source: [Kaggle - Brain MRI Images for Brain Tumor Detection](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri)
- Classes:
  - `yes` → Tumor Type (glioma, meningioma, pituitary)
  - `no` → No Tumor
- Format: `.jpg` MRI images

---

## Model Architecture

> Here's a summary of the CNN architecture used:

```python
Conv2D(32) → ReLU → MaxPooling  
Conv2D(64) → ReLU → MaxPooling  
Conv2D(128) → ReLU → MaxPooling  
Flatten → Dense(128) → Dropout  
Output Layer (Softmax or Sigmoid)
