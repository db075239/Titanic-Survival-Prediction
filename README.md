# 🚢 Titanic Survival Prediction

Welcome to my take on the well-known **Kaggle Titanic Machine Learning Challenge**. This project explores a variety of machine learning models and techniques to predict passenger survival aboard the Titanic — one of the most well-known tragedies in modern history.

---

## 🧭 Table of Contents
- [📌 Introduction](#-introduction)
- [🎯 Project Goal](#-project-goal)
- [🧾 Dataset](#-dataset)
- [⚙️ Methodology](#-methodology)
- [🤖 Models Implemented](#-models-implemented)
- [📊 Results](#-results)
- [📁 Files in this Repository](#-files-in-this-repository)
- [📝 Conclusion](#-conclusion)

---

## 📌 Introduction

The **Titanic dataset** is a classic benchmark in the field of data science and machine learning. Its real-world significance and relatively well-structured data make it perfect for introducing and demonstrating core ML concepts.

This project applies a full machine learning pipeline — from preprocessing to model evaluation — to solve a **binary classification problem**: predicting survival on the Titanic.

---

## 🎯 Project Goal

The objective is to **predict whether a given passenger survived** the Titanic disaster based on personal and travel-related attributes.  
This is a supervised classification task with two possible outcomes:
- **1**: Survived
- **0**: Did not survive

---

## 🧾 Dataset

The dataset is sourced from [Kaggle’s Titanic Challenge](https://www.kaggle.com/competitions/titanic). It includes demographic and socio-economic details of Titanic passengers.

Key features include:
- `Age`
- `Sex`
- `Fare`
- `Pclass` (Ticket Class)
- `SibSp`, `Parch` (Family relationships)
- `Embarked`, `Cabin`, `Ticket` and more.

### 🗂 Files
- `train.csv` — For training and validating models.
- `test.csv` — For evaluating model predictions on unseen data.

---

## ⚙️ Methodology

A typical machine learning workflow was followed:

1. **🧹 Data Preprocessing**
   - Imputation of missing values
   - Label encoding for categorical variables
   - Feature engineering (e.g., `FamilySize`, `IsAlone`)
2. **⚖️ Feature Scaling**
   - Standardization to ensure balanced input for distance-based models like KNN.
3. **🧠 Model Implementation**
   - Training multiple ML algorithms to compare their performance.
4. **📈 Model Evaluation**
   - Using metrics like accuracy, precision, recall, and confusion matrix to measure effectiveness.

---

## 🤖 Models Implemented

Three machine learning algorithms were trained and compared:

- **🔹 Logistic Regression**
  - A simple yet powerful linear model for binary classification.
  - Pros: Interpretable and fast.
  
- **🌲 Random Forest**
  - An ensemble of decision trees; handles overfitting better.
  - Pros: High accuracy and robust performance.

- **👥 K-Nearest Neighbors (KNN)**
  - A lazy learning algorithm that classifies based on proximity in feature space.
  - Pros: Performs well with properly scaled data.

---

## 📊 Results

The models delivered promising results, with **Random Forest** outperforming others overall.

| Model               | Accuracy | Notes                          |
|--------------------|----------|--------------------------------|
| **Random Forest**   | ✅ High   | Best balance of accuracy and robustness |
| **KNN**             | ✅ Good   | Improved with scaling          |
| **Logistic Regression** | ✔️ Moderate | Simple and interpretable       |

> 🔍 Feature engineering (e.g., combining `SibSp` and `Parch`) and scaling significantly improved performance.

---

## 📁 Files in this Repository

| File | Description |
|------|-------------|
| `Projekt.ipynb` | The main Jupyter Notebook with the full pipeline: data loading, preprocessing, training, and evaluation. |
| `AIS_Report.pdf` | A detailed written report covering methodology, background theory, and results. |
| `train.csv` | Training data for the Titanic challenge. |
| `test.csv` | Test data for final predictions. |

---

## 📝 Conclusion

This project successfully demonstrates how classic machine learning techniques can be applied to real-world problems. It reinforces the importance of:
- Data preprocessing
- Feature scaling and engineering
- Model comparison and evaluation

### 🚀 Future Work
To further improve performance, future enhancements could include:
- Feature extraction from `Cabin` and `Ticket` fields
- Ensemble stacking or boosting (e.g., XGBoost, LightGBM)
- Incorporating deep learning models for comparison

---

> *"A smooth sea never made a skilled sailor."*  
> ― Franklin D. Roosevelt

---
