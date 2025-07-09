# Titanic Survival Prediction

This is my take, my try on the very well-known challenge on Kaggle: predicting passenger survival on the Titanic. This project explores various machine learning models and techniques to build a robust predictor for one of history's most tragic events.

## Table of Contents

* [Introduction](#introduction)
* [Project Goal](#project-goal)
* [Dataset](#dataset)
* [Methodology](#methodology)
* [Models Implemented](#models-implemented)
* [Results](#results)
* [Files in this Repository](#files-in-this-repository)
* [Conclusion](#conclusion)

## Introduction

The Titanic dataset is a classic for introducing machine learning concepts due to its relatively clean data and compelling historical context. This project aims to demonstrate the application of machine learning principles, from data preprocessing to model evaluation, in a binary classification problem.

## Project Goal

The primary goal of this project is to predict whether a passenger survived the Titanic disaster based on a set of provided features. This is a binary classification task where the output is either "survived" or "did not survive".

## Dataset

The dataset used for this project is the famous Titanic dataset, available on Kaggle. It contains information about passengers, including:
* Age
* Gender
* Fare
* Ticket Class
* Other attributes relevant to survival prediction.

The raw data is split into two files:
* `train.csv`: Used for training the machine learning models.
* `test.csv`: Used for making predictions and evaluating the model's performance on unseen data.

## Methodology

The project followed a standard machine learning pipeline:
1.  **Data Preprocessing**: Handling missing values, encoding categorical features, and transforming data to be suitable for model training.
2.  **Feature Scaling**: Applying scaling techniques to ensure that features contribute equally to the model's performance, especially for distance-based algorithms.
3.  **Model Implementation**: Training and tuning various machine learning algorithms.
4.  **Model Evaluation**: Assessing model performance using metrics such as accuracy, precision, and recall.

## Models Implemented

Three different machine learning models were implemented and compared in this project:
* **Logistic Regression**: A linear model used for binary classification. It provides interpretable results.
* **Random Forest**: An ensemble learning method that builds multiple decision trees and merges their predictions to improve accuracy and control overfitting.
* **K-Nearest Neighbors (KNN)**: A non-parametric, lazy learning algorithm that classifies new data points based on the majority class of their 'k' nearest neighbors.

## Results

The project demonstrated that machine learning algorithms can effectively predict survival outcomes. Among the implemented models:
* **Random Forest** emerged as the most robust model, achieving a good balance between precision and recall.
* **KNN** performed well in terms of overall accuracy, particularly when applied to scaled features.
* **Logistic Regression**, while slightly less accurate, provided consistent and interpretable results.

Feature scaling and selection significantly impacted the model's performance, highlighting their importance in the preprocessing phase.

## Files in this Repository

* `Projekt.ipynb`: The main Jupyter Notebook containing the complete code for data loading, preprocessing, model implementation, training, evaluation, and visualization. This is where the core analysis takes place.
* `AIS_Report.pdf`: The detailed project report (in English), providing an in-depth explanation of the methodology, theoretical background, results, and conclusions. This document supplements the code with comprehensive insights.
* `train.csv`: The training dataset for the Titanic challenge.
* `test.csv`: The test dataset for the Titanic challenge.

## Conclusion

This project successfully applied various machine learning techniques to the Titanic survival prediction problem. It showcases a practical understanding of data preprocessing, model selection, and performance evaluation. Future enhancements could include exploring additional features like family size and cabin location, or experimenting with more advanced models like Gradient Boosting or Neural Networks.
