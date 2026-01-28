# 🎒 Backpack Price Prediction Challenge

## Overview
This project focuses on predicting backpack prices using supervised machine learning.  
The goal is to capture non-linear price patterns through careful preprocessing, feature engineering, and ensemble models.

The project was developed in **Jupyter Notebook**.

---

## Dataset
The dataset was generated using a deep learning model trained on the *Student Bag Prediction* dataset.  
Feature distributions are similar but not identical, adding complexity to the prediction task.

**Files:**
- `train.csv` – training data with target variable (`Price`)
- `train_extra.csv` – additional training data
- `test.csv` – test set for prediction
- `sample_submission.csv` – submission format

---

## Methodology
- Log transformation applied to the target variable
- Top and bottom **1% outliers removed**
- Missing values handled via imputation, binary encoding, and label encoding
- Feature distribution analysis and normalization

---

## Models & Performance
Models evaluated:
- Linear Regression
- Decision Trees
- Gradient Boosting
- XGBoost

**Key results:**
- Ensemble models (XGBoost, Gradient Boosting) outperformed linear models
- Linear models struggled with non-linearity (R² ≈ 0.0003)
- After preprocessing:
  - **RMSE ≈ 38.5**
  - **MAE ≈ 33.28**

---

## Insights
- Backpack prices show high variance and non-linear behavior
- Outlier removal significantly improved model stability
- Using `train_extra.csv` provided small but meaningful performance gains

---

## Conclusion
XGBoost and Gradient Boosting are the most suitable models for this task.  
The project highlights the importance of data quality and ensemble learning in real-world price prediction.

---

## Tools
Python, Pandas, NumPy, Scikit-learn, XGBoost, Jupyter Notebook
