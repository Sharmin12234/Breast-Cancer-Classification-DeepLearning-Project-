
# Breast Cancer Histopathology Image Classification 🧬

This project uses Deep Learning to detect breast cancer from biopsy images. It classifies tissue samples into two categories: **Benign** (non-cancerous) and **Malignant** (cancerous).

## 📋 Project Overview
I used the **BreaKHis v1** dataset and implemented **Transfer Learning** with the **ResNet50** architecture. The goal is to automate the screening process of histopathology slides.

## 🛠 Tech Stack
- **Deep Learning:** TensorFlow & Keras
- **Architecture:** ResNet50 (Pre-trained)
- **Libraries:** NumPy, Pandas, Matplotlib, Seaborn
- **Preprocessing:** ImageDataGenerator (Data Augmentation)

## 📊 Dataset Info
The dataset contains microscopic images of breast tumor tissue:
- **Benign:** Non-harmful tumors (Adenosis, Fibroadenoma, etc.)
- **Malignant:** Cancerous tumors (Carcinoma, Papillary Carcinoma, etc.)

## 🚀 Model Details
1. **Input Size:** 224x224 pixels.
2. **Method:** Initially trained the top layers, followed by fine-tuning the base ResNet50 model.
3. **Optimizers:** Adam optimizer with custom learning rates.
4. **Callbacks:** Used `EarlyStopping` and `ModelCheckpoint` to save the `final_best_model.h5`.

## 📈 Evaluation
The project includes a confusion matrix and classification report to evaluate the performance of the model on unseen test data.

---
*Uploaded as part of my 1-year data science learning journey.*