# 🔍 SHAP Neural Network XAI

## 📌 Overview

This project demonstrates the use of **Explainable Artificial Intelligence (XAI)** to explain predictions made by a **Neural Network** using **SHAP (SHapley Additive exPlanations)**.

A neural network is trained on the **Breast Cancer Wisconsin dataset** to classify tumors into two classes: **Malignant** and **Benign**. After training the model, SHAP is applied to understand which input features contribute to the model's predictions.

The project demonstrates both **global** and **local** explanations of neural-network predictions.

---

## 🎯 Objectives

- Build a neural-network classification model.
- Train the model using the Breast Cancer Wisconsin dataset.
- Preprocess and standardize the input features.
- Evaluate the performance of the trained model.
- Apply SHAP to the neural network.
- Identify important features influencing predictions.
- Explain an individual prediction using a SHAP waterfall plot.
- Understand how explainability supports transparency, fairness, accountability, and trust in AI.

---

## 🗂️ Dataset

The project uses the **Breast Cancer Wisconsin dataset** available through Scikit-learn.

### Dataset Details

| Property | Value |
|---|---:|
| Total Samples | 569 |
| Number of Features | 30 |
| Training Samples | 455 |
| Testing Samples | 114 |
| Number of Classes | 2 |
| Classes | Malignant / Benign |

The dataset contains numerical features describing characteristics of cell nuclei obtained from breast-cancer samples.

Some of the features include:

- Mean Radius
- Mean Texture
- Mean Perimeter
- Mean Area
- Mean Smoothness
- Mean Compactness
- Mean Concavity
- Mean Concave Points
- Radius Error
- Texture Error
- Perimeter Error
- Area Error
- Worst Radius
- Worst Texture
- Worst Perimeter
- Worst Area
- Worst Smoothness
- Worst Compactness
- Worst Concavity
- Worst Concave Points

---

## 🧠 Neural Network Architecture

The neural network was implemented using **TensorFlow/Keras**.

```text
                 Input Layer
                 30 Features
                      │
                      ▼
              Dense Layer
              64 Neurons
                ReLU
                      │
                      ▼
              Dense Layer
              32 Neurons
                ReLU
                      │
                      ▼
              Output Layer
               1 Neuron
               Sigmoid
                      │
                      ▼
             Model Prediction
