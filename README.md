# 🧠 ResNet From Scratch – CIFAR-10 Classification

This project implements **Residual Networks (ResNet)** entirely from scratch using **TensorFlow/Keras**, and applies them to the CIFAR-10 image classification task. A custom-built ResNet-18 architecture is used to balance **performance and training time**, achieving strong classification results and insightful predictions.

---

## 🚀 Highlights

- ✅ Implemented **ResNet blocks and full ResNet architecture** from scratch.
- ✅ Trained on the **CIFAR-10 dataset** (32x32 RGB images).
- ✅ Compared different ResNet depths: **ResNet-18, 34, 50**.
- ✅ Visualized **Top-5 class predictions** with confidence bars.
- ✅ Final version uses **ResNet-18** for optimal trade-off between accuracy and training time.

---

## 🏗️ ResNet Architecture

Implemented components:
- 🔹 Convolutional Blocks with BatchNorm + ReLU
- 🔹 Identity and Projection Shortcuts
- 🔹 Residual Block Builder Function
- 🔹 Final Fully Connected Classifier

Supported architectures:
- `ResNet-18` ✅ (used in final model)
- `ResNet-34`, `ResNet-50` (tested, slower, high memory)

---

## 🧪 Model Performance

| Metric                | Score     |
|-----------------------|-----------|
| ✅ Training Accuracy   | **95.15%** |
| ✅ Validation Accuracy | **89.82%** |
| ✅ Top-5 Accuracy      | **99.64%** |

- Optimizer: `Adam`
- Loss: `SparseCategoricalCrossentropy`
- EarlyStopping + ModelCheckpoint used

---

## 📊 Top-5 Class Predictions Demo

Images can be uploaded for prediction using the trained ResNet model. The model displays top-5 labels with confidence bars for each image.

## 🧠 Why ResNet-18?

While ResNet-50 and deeper models perform better in theory, on CIFAR-10 they led to:
- ⚠️ **High computation time**
- ⚠️ **Overfitting**
- ⚠️ **GPU memory issues (on Colab)**

Hence, **ResNet-18** was chosen for:
- ⚡ Faster training
- 🔄 Balanced depth
- 🧠 Sufficient representation for CIFAR-10

---
