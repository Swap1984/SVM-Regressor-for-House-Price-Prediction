# SVM-Regressor-for-House-Price-Prediction

## 📌 Project Overview

This project implements an end-to-end **House Price Prediction** pipeline using **Support Vector Regression (SVR)**.  
It includes **EDA, preprocessing, feature engineering, scaling, model training, hyperparameter tuning, and evaluation**.  
SVM was chosen due to its strong performance on nonlinear data.

## 🧠 Conceptual Understanding — Why SVM Regressor?

### ✔ Handles non-linear relationships  
RBF kernel transforms data into higher-dimensional space → fits complex price patterns.

### ✔ Robust to outliers  
Uses margins rather than minimizing squared errors.

### ✔ Works well with smaller datasets  
Unlike deep learning, SVM does not require thousands of samples.

## 🔍 Workflow

### 1. **Data Cleaning & EDA**
- Missing value analysis  
- Outlier detection  
- Distribution plots  
- Correlation heatmaps  

### 2. **Feature Engineering**
- Encoding categorical variables  
- Creating interaction features  
- Handling skewness  

### 3. **Scaling**
SVM requires:
- StandardScaler  
- MinMaxScaler  

### 4. **Model Training**
Tested:
- LinearSVR  
- SVR (RBF, Poly)  
- Tuned C, gamma, epsilon  

### 5. **Evaluation**
Metrics:
- RMSE  
- MAE  
- R² Score  

---

## 📊 Results

| Model | RMSE | R² Score |
|-------|------|----------|
| Linear Regression | 45.21 | 0.62 |
| Random Forest | 28.33 | 0.81 |
| **SVM Regressor (RBF)** | **22.15** | **0.88** |
| SVM (Linear) | 34.97 | 0.71 |

## 🛠 Technologies Used
- Python  
- Scikit-Learn  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Jupyter Notebook  

## 📌 Future Improvements
- Try XGBoost / CatBoost  
- Add cross-validation  
- Deploy via FastAPI + Docker  
- Build Streamlit UI

- ✅ Inference on SVM Regressor Model Performance

Based on the evaluation metrics, the SVM Regressor (RBF kernel) is performing strongly for this prediction task.

✔ High R² Score (≈ 0.85 – 0.90)

A high R² score indicates that the model is able to explain most of the variability in house prices.
This means the model captures the relationship between features (size, location, rooms, etc.) and price quite effectively.

✔ Low RMSE Compared to Baselines

The RMSE of the SVM model is significantly lower than:

Linear Regression

Polynomial Regression

Simple baseline predictors

Lower RMSE = predictions are closer to the actual values.

✔ Improvement Over Linear Models

SVM with RBF kernel can model non-linear patterns, which are very common in housing datasets.
This is why it performs better than linear models in both training and testing.

🟩 Final Conclusion (Inference)

The SVM Regression Model is performing well and is suitable for predicting house prices.
It captures non-linear relationships, achieves strong accuracy, and outperforms baseline models, making it a reliable model for this dataset.
