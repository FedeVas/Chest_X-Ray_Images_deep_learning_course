# 🩻 Chest X-Ray Pneumonia Detection — Deep Learning Course (MIPT)

This repository contains the final exam project for the **Deep Learning in Data Science** course at **MIPT (Moscow Institute of Physics and Technology)**.

📁 **Dataset**:  
Chest X-Ray Images (Pneumonia) — [Kaggle Link](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)

---

## 📌 Project Structure

- `EDA_and_Models.ipynb` — Full notebook containing:
  - Exploratory Data Analysis (EDA)
  - Data preprocessing and augmentation
  - Baseline CNN model (≤1M parameters)
  - Improved model using Transfer Learning (MobileNetV2)
  - Evaluation and comparison of both models

- `README.md` — Project overview and usage instructions

---

## 📊 Task Overview

The goal of the project is to classify chest X-ray images into two categories:
- **NORMAL**
- **PNEUMONIA**

The task is solved in three stages:
1. **Data exploration and preprocessing**
2. **Training a simple custom CNN (≤1M params)**
3. **Training an improved model using transfer learning**

---

## ✅ Results Summary

| Metric            | Baseline CNN | MobileNetV2 (Transfer Learning) |
|-------------------|--------------|----------------------------------|
| Accuracy          | 0.77         | 0.82                             |
| Recall (PNEUMONIA)| 0.71         | **0.99**                         |
| ROC-AUC           | 0.871        | **0.963**                        |

📈 Transfer learning led to a **+9.2% gain in ROC-AUC**, and significantly improved sensitivity to pneumonia cases.

---

## 🚀 How to Run

1. Clone the repository or download the `.ipynb` file.
2. Run the notebook on:
   - **Kaggle** (recommended)
   - **Google Colab**
   - Any local Jupyter environment with TensorFlow 2.x

3. Download the dataset from Kaggle and place it in a `data/` folder:
```bash
kaggle datasets download -d paultimothymooney/chest-xray-pneumonia
unzip chest-xray-pneumonia.zip -d data/
```

## 🧠 Author
Vasilii Fede
Deep Learning Course — MIPT, June 2025
Project submitted as part of final assessment.

📜 License
This project is released for educational use. All image data belongs to their respective sources (see [Kaggle license](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)).
