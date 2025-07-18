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

##  How to Use

1. **Clone this repository**
   ```bash
   git clone https://github.com/yourusername/return-risk-prediction.git
   cd return-risk-prediction
