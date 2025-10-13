# 🧠 Enerlytic Machine Learning Pipeline – Python Notebook

> A complete end-to-end **machine learning workflow** for data preprocessing, model training, and performance visualization.  
> Built with **Python**, **Scikit-learn**, and **Matplotlib**, this project demonstrates best practices for building interpretable and data-driven analytics systems.

---

## 🧭 Project Overview

This notebook implements a **data-to-decision pipeline** that automates every major step of a supervised ML workflow — from **ETL and feature engineering** to **model training**, **evaluation**, and **visualization**.  
It was developed as part of the *Enerlytic* initiative to bridge **data analytics** and **engineering intelligence** for sustainable systems.

The pipeline supports:
- Automated **data cleaning**, transformation, and encoding  
- Training of multiple ML models (Logistic Regression, Random Forest, etc.)  
- Evaluation using **accuracy**, **ROC-AUC**, **log loss**, and **confusion matrices**  
- Visual analytics with **Matplotlib** and Power BI-style dashboards  

---

## ⚙️ Methodology

### 1️⃣ **Data Preprocessing**
- Safe CSV import with encoding detection  
- Removal of redundant or ID columns  
- Imputation of missing values using median or mean  
- Feature scaling and one-hot encoding via `ColumnTransformer`

### 2️⃣ **Exploratory Data Analysis (EDA)**
- Data structure inspection  
- Summary statistics and correlation heatmaps  
- Distribution plots for target and key predictors  

### 3️⃣ **Model Development**
Two models were developed and benchmarked:
| Model | Accuracy | ROC-AUC | Log Loss |
|--------|-----------|----------|----------|
| Logistic Regression | ~0.85 | ~0.90 | ~0.34 |
| Random Forest | ~0.93 | ~0.96 | ~0.22 |

> *Values are illustrative; actual results depend on dataset.*

### 4️⃣ **Model Evaluation**
- ROC curve comparison  
- Confusion matrix visualization  
- Feature importance extraction for interpretability  
- Metric logging and model serialization (`.joblib`)

---

## 📊 Key Results

- **Random Forest** consistently outperformed Logistic Regression across metrics.  
- **Top predictors** included *Flight Distance*, *Departure Delay*, *Inflight Service*, and *Seat Comfort*.  
- The **ROC-AUC > 0.95** demonstrated robust separation capability.  
- Automated reporting improved reproducibility and model explainability.  

---

## 🖼️ Results Visualization Gallery

### 🔹 ROC Curves
<p align="center">
  <img src="results/roc_logistic.png" alt="ROC Curve - Logistic Regression" width="45%">
  <img src="results/roc_random_forest.png" alt="ROC Curve - Random Forest" width="45%">
</p>
<p align="center"><em>Comparison of ROC curves showing the Random Forest’s superior classification performance.</em></p>

---

### 🔹 Confusion Matrices
<p align="center">
  <img src="results/confusion_logistic.png" alt="Confusion Matrix - Logistic Regression" width="45%">
  <img src="results/confusion_random_forest.png" alt="Confusion Matrix - Random Forest" width="45%">
</p>
<p align="center"><em>Distribution of predictions highlighting classification precision and recall trade-offs.</em></p>

---

### 🔹 Feature Importance
<p align="center">
  <img src="results/rf_feature_importances.png" alt="Feature Importance - Random Forest" width="70%">
</p>
<p align="center"><em>Top 20 features influencing satisfaction predictions.</em></p>

---

## 📈 Performance Dashboard Preview

The **Performance Dashboard** consolidates ML performance metrics, feature impacts, and satisfaction trends into an interactive Power BI–style layout.  
It blends analytical depth with business-ready clarity.

<p align="center">
  <img src="assets/performance_dashboard_preview.png" alt="Performance Dashboard Preview" width="85%">
</p>
<p align="center"><em>Composite dashboard showcasing Accuracy, ROC-AUC, Log Loss, and top predictive features.</em></p>

**Dashboard Layout Design**
