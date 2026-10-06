<div align="center">

# 🐱🐶 Cat vs Dog Image Classification

**A CNN-based binary image classifier built with TensorFlow/Keras, reaching 98% test accuracy.**

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-FF6F00?logo=tensorflow&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikit-learn&logoColor=white)
![Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?logo=googlecolab&logoColor=white)
![Accuracy](https://img.shields.io/badge/Test%20Accuracy-98%25-brightgreen)

[Open in Colab](<your-colab-link>) · [Report Bug](<your-repo-link>/issues)

</div>

---

## 📌 Overview

This project trains a Convolutional Neural Network (CNN) from scratch to classify images as either a **cat** or a **dog**. It covers the full workflow: data splitting, augmentation, model building, training, and evaluation with per-class metrics.

## ✨ Highlights

- Custom 3-block CNN with **Batch Normalization** and **Dropout** for stable training and regularization
- **Data augmentation** to improve generalization on a small dataset
- Balanced dataset with a clean **70 / 15 / 15** train / validation / test split
- **98% test accuracy** with strong precision and recall for both classes

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| Deep Learning | TensorFlow, Keras |
| Data & Math | NumPy |
| Visualization | Matplotlib |
| Evaluation | Scikit-learn |
| Environment | Google Colab |

## 🧠 Model Architecture

```text
Input (128 × 128 × 3)
        ↓
Data Augmentation
        ↓
Rescaling (1/255)
        ↓
Conv2D (32)  → BatchNorm → ReLU → MaxPooling
        ↓
Conv2D (64)  → BatchNorm → ReLU → MaxPooling
        ↓
Conv2D (128) → BatchNorm → ReLU → MaxPooling
        ↓
Flatten
        ↓
Dense (128) → BatchNorm → ReLU
        ↓
Dropout (0.5)
        ↓
Dense (1) → Sigmoid
        ↓
Cat / Dog
```

## 📂 Dataset

| Class | Images |
|---|---|
| Cats | 500 |
| Dogs | 500 |
| **Total** | **1,000** |

| Split | Share |
|---|---|
| Training | 70% |
| Validation | 15% |
| Testing | 15% |

> Dataset source: `<add dataset name / link>`

## 📊 Results

**Test Accuracy: 98%**

| Class | Precision | Recall | F1-Score |
|---|:---:|:---:|:---:|
| Cat | 0.96 | 1.00 | 0.98 |
| Dog | 1.00 | 0.96 | 0.98 |

The model never misclassifies a cat, and every image it labels as a dog is truly a dog. Its few errors are dogs predicted as cats.



## 👤 Author

Debasish Ghosh




---

<div align="center">⭐ If you found this useful, consider starring the repo!</div>
