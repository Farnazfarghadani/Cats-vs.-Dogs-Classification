# Cats vs Dogs Classification with MobileNetV2

This project classifies cat and dog images using transfer learning with MobileNetV2, achieving **98% accuracy** on the validation set.

---

##Dataset

- Source: [Kaggle Dogs vs. Cats](https://www.kaggle.com/c/dogs-vs-cats/data)
- Structure:
dataset/
├── train/
│ ├── cats/
│ └── dogs/
└── test/
├── cats/
└── dogs/

---

---

##Model

- **Base Model**: `MobileNetV2` (pre-trained on ImageNet)
- **Image Size**: `224 x 224`
- **Data Augmentation**: Yes
- **Fine-Tuning**: Yes (last 20 layers)
- **Class Balancing**: Yes (using `class_weight`)
- **Accuracy**: `98%`

---

##Results

- **Confusion Matrix**:

Classification Report:
              precision    recall  f1-score   support

        cats       0.98      0.98      0.98      3177
        dogs       0.97      0.96      0.97      1846

    accuracy                           0.98      5023
   macro avg       0.98      0.97      0.98      5023
weighted avg       0.98      0.98      0.98      5023

---
##Requirements:

tensorflow
scikit-learn
matplotlib
numpy
