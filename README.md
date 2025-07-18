#  Intelligent Return Risk Prediction System (XGBoost-Based)

This project implements a machine learning system to **predict the likelihood of product returns** in an e-commerce setting. The model is trained on transactional data and leverages the power of **XGBoost** combined with **SMOTE** and **threshold tuning** to handle class imbalance and improve return detection.

---

##  Problem Statement

In e-commerce, product returns are costly. Predicting which orders are likely to be returned helps businesses:
- Reduce reverse logistics costs
- Improve customer satisfaction
- Make smarter inventory and marketing decisions

---

##  Dataset Columns

| Column Name   | Description                  |
|---------------|------------------------------|
| `order_id`    | Unique identifier for order  |
| `product_id`  | Unique product identifier    |
| `price`       | Price of the product         |
| `rating`      | Customer rating (1–5 scale)  |
| `return_status` | Target variable (1 = Returned, 0 = Not Returned) |

---

## ⚙ Methods Used

- **XGBoost Classifier** for robust and scalable classification
- **Label Encoding** for categorical feature (`product_id`)
- **SMOTE (Synthetic Minority Over-sampling Technique)** to balance class 1 (returned)
- **Threshold tuning** to improve recall on return predictions
- **Confusion Matrix** and **Classification Report** for evaluation

---

<!-- PROJECT SHIELDS -->
<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/status-production-green.svg" alt="Status"></a>
  <a href="#"><img src="https://imgields.io/badge/python-3.8%2B-blue.svg" alt="Python Version"></a>
  <a href="#license"><img src="https://imgields.io/badge/license-MIT-blue.svg" alt="License"></a>
</p>

# Intelligent Return Risk Prediction System

High-impact, scalable machine learning solution for forecasting product return likelihood in e-commerce. By combining **XGBoost**, **SMOTE**, and **threshold optimization**, this system delivers actionable insights to reduce operational costs and enhance customer satisfaction.

---

## 🚀 Features

- **Imbalanced Data Handling**: SMOTE oversampling + `scale_pos_weight` ensure balanced learning.
- **High-Performance Modeling**: XGBoost classifier with optimized parameters for structured data.
- **Custom Threshold Tuning**: Maximize recall on return predictions to capture true positives.
- **Modular Codebase**: Clear separation of data processing, modeling, and evaluation.
- **Easy Integration**: Single script interface and exportable model for deployment.

---

## 🗂 Tech Stack

- **Language**: Python 3.8+
- **ML Frameworks**: XGBoost, scikit-learn, imbalanced-learn
- **Visualization**: Matplotlib
- **Data Handling**: pandas, NumPy

---

## 📊 Project Structure
├── data/
│ └── return_data.csv # Sample dataset
├── src/
│ ├── return_risk_prediction.py # Main script
│ └── utils.py # Helper functions
├── notebooks/ # EDA and experimentation
├── requirements.txt
└── README.md # Project overview

##Acknowledgements

XGBoost, scikit-learn, and imbalanced-learn communities
Dataset contributors and e-commerce domain experts
