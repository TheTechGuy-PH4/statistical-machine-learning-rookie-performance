# Statistical Machine Learning – Rookie Performance Prediction

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Neural%20Networks-FF6F00.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)
![License](https://img.shields.io/badge/License-Educational-blue)

---

# Overview

This repository contains my graduate Statistical Machine Learning research project completed as part of my Master's degree in **Robotics and Autonomous Systems (Artificial Intelligence)** at **Arizona State University**.

The objective was to investigate whether machine learning models can accurately predict **NFL rookie fantasy football performance** using only information available before a player enters the league.

Rather than building a production fantasy football tool, the project evaluates how different statistical learning algorithms perform on structured sports data while demonstrating the complete machine learning workflow:

- Data collection
- Data preprocessing
- Exploratory Data Analysis
- Supervised Learning
- Unsupervised Learning
- Model Evaluation
- Feature Importance
- Future Predictions

The project culminated in an IEEE-style research paper and prediction model for the 2026 rookie class.

---

# Research Objectives

The project investigates two separate machine learning problems.

## Regression

Predict a player's total rookie season PPR fantasy points.

Output:

```
Predicted Rookie PPR Points
```

---

## Classification

Predict whether a rookie becomes **Fantasy Relevant** based upon position-specific thresholds.

Examples:

- QB → Top 12
- RB → Top 24
- WR → Top 36
- TE → Top 12

Output:

```
Fantasy Relevant
Yes / No
```

---

# Dataset

The dataset was manually constructed using publicly available NFL draft and college statistics.

Player features include:

- Draft Position
- Age
- Height
- Weight
- College Games
- College Yards
- College Touchdowns
- Position

Historical rookie classes were used for training and testing before generating predictions for the 2026 draft class.

---

# Repository Structure

```
statistical-machine-learning-rookie-performance/

│
├── Project Phase - PDFs/
│
├── Final Report HTML/
│
├── data/
│   └── processed/
│
├── 01_phase2_data_validation.ipynb
├── 02_phase3_eda.ipynb
├── 03_phase4_baseline_models.ipynb
├── 04_phase5_tree_models.ipynb
├── 05_phase6_neural_networks.ipynb
├── 06_phase7_explainability_unsupervised.ipynb
├── 07_phase8_2026_predictions.ipynb
│
├── Fantasy-Lord-Rookie-ML-Dataset.xlsx
├── 2026_rookie_predictions.xlsx
│
└── README.md
```

---

# Machine Learning Pipeline

```
Raw Player Data
        │
        ▼
Data Validation
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Feature Engineering
        │
        ▼
Train / Test Split
        │
        ▼
Baseline Models
        │
        ▼
Tree Models
        │
        ▼
Neural Networks
        │
        ▼
Model Evaluation
        │
        ▼
Feature Importance
        │
        ▼
PCA + KMeans
        │
        ▼
2026 Rookie Predictions
```

---

# Models Implemented

## Baseline Models

- Linear Regression
- Logistic Regression

---

## Tree-Based Models

- Decision Tree Regressor
- Decision Tree Classifier
- Random Forest Regressor
- Random Forest Classifier

---

## Deep Learning

- Feedforward Neural Network
- Early Stopping Comparison

---

## Unsupervised Learning

- Principal Component Analysis (PCA)
- K-Means Clustering

---

# Evaluation Metrics

Regression

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

Classification

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

---

# Key Results

## Best Classification Model

Random Forest Classifier

ROC-AUC

```
≈ 66%
```

---

## Best Regression Model

Random Forest Regressor

RMSE

```
≈ 94 Fantasy Points
```

---

## Major Findings

✔ Random Forest consistently outperformed all other supervised learning models.

✔ Neural Networks overfit due to the relatively small structured dataset.

✔ Draft Capital was the strongest predictor of total fantasy production.

✔ College production metrics were stronger predictors of fantasy relevance.

✔ PCA revealed natural positional separation.

✔ K-Means identified distinct rookie archetypes.

---

# Feature Importance

The Random Forest models revealed two interesting insights.

Regression:

- Draft Position dominated prediction importance.

Classification:

- College Yards
- College Touchdowns

became the strongest indicators of fantasy relevance.

---

# 2026 Rookie Predictions

After selecting the best-performing Random Forest models, predictions were generated for the 2026 rookie class.

Outputs include:

- Predicted Rookie PPR Points
- Fantasy Relevance Probability
- Position
- Classification Prediction

This demonstrates how historical machine learning models can be extended to future draft classes.

---

# Technologies Used

Programming

- Python

Machine Learning

- Scikit-Learn
- TensorFlow

Data Analysis

- Pandas
- NumPy

Visualization

- Matplotlib
- Seaborn

Development

- Jupyter Notebook

Version Control

- Git
- GitHub

---

# Skills Demonstrated

This project demonstrates experience with:

- Statistical Machine Learning
- Regression
- Classification
- Feature Engineering
- Data Validation
- Data Preprocessing
- Model Comparison
- Random Forests
- Neural Networks
- Explainable AI
- PCA
- K-Means
- Hyperparameter Evaluation
- Overfitting Analysis
- Technical Research Writing

---

# Future Improvements

Potential future work includes:

- Expand the dataset to 400+ players
- Include offensive line quality
- Team offensive efficiency
- Coaching tendencies
- Strength of schedule
- Opportunity metrics
- Reinforcement Learning for dynasty draft optimization
- SHAP explainability
- XGBoost and LightGBM comparison
- Ensemble learning methods

---

# Research Paper

The complete IEEE research paper describing the methodology, experiments, and results is included in this repository.

Topics include:

- Problem Formulation
- Dataset Construction
- Statistical Learning Methods
- Model Comparison
- Neural Network Analysis
- Feature Importance
- PCA & Clustering
- 2026 Rookie Predictions
- Future Work

---

# About Me

**Phillip Hogan**

M.S. Robotics & Autonomous Systems (Artificial Intelligence)

Arizona State University

My long-term goal is to become a **Humanoid Robotics Engineer**, building intelligent robotic systems that integrate machine learning, reinforcement learning, embedded systems, software engineering, and mechanical design.

GitHub:
https://github.com/TheTechGuy-PH4

LinkedIn:
https://linkedin.com/in/phillip-a-hogan

---

# License

This repository is intended for educational and portfolio purposes.

The project was completed as graduate coursework at Arizona State University and is shared to demonstrate machine learning methodology, software engineering practices, and technical research writing.
