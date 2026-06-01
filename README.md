# Hybrid Machine Learning and Reinforcement Learning System for Road Safety

A machine learning system that predicts road accident risk and recommends safety interventions using classification models and Q-Learning reinforcement learning. Built using South African road accident data (2017)

## Overview

This project combines supervised machine learning and reinforcement learning to:

Predict whether a road segment/scenario is high or low risk for accidents
Recommend the best road safety policy (e.g., deploying speed cameras) using a Q-Learning agent

## Models Used 
Random Forrest
XGBoost
Q-Learning(RL)

  
##  Methodology

### 1. Data Preprocessing
- Cleaning missing and inconsistent values
- Encoding categorical variables
- Normalising numerical features
- Exploratory Data Analysis (EDA) to identify patterns

### 2. Machine Learning Models
The following models were implemented and compared:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost 

Evaluation metrics:
- Accuracy
- Precision
- Recall
- F1-score


---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- Matplotlib
- Reinforcement Learning (Q-Learning)

## Features

- Data preprocessing and cleaning
- Random Forest classification
- XGBoost classification
- Model evaluation metrics
- Confusion matrix analysis
- Markov Decision Process (MDP)
- Q-Learning implementation
- Policy evaluation

## Results
Classification Models
Random Forest achieved perfect classification on the test set correctly identifying all high-risk and low-risk cases with zero misclassifications.
XGBoost achieved ~96% accuracy, misclassifying 1 out of 6 positive (high-risk) cases.
Reinforcement Learning (Q-Learning)
The Q-Learning agent was trained to recommend road safety policies based on predicted risk states:

Low risk state -> No_Action
Medium/High risk state -> Speed_Cameras

The agent's Q-values converged rapidly within ~100 episodes, stabilising near the maximum reward value of 100.




## Dataset
South Africa Road Accidents Dataset – 2017
Contains historical road accident records used for binary risk classification (accident / no accident).
Kaggle-https://www.kaggle.com/datasets/velile/car-accidents

***This project is for educational and portfolio purposes.
