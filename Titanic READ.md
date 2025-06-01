# Titanic Survival Prediction

This repository contains a machine learning project that predicts survival outcomes for passengers on the Titanic using the classic Titanic dataset. The dataset is analyzed, cleaned, visualized, and used to train classification models.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Preprocessing](#data-preprocessing)
- [Modeling](#modeling)
- [Hyperparameter Tuning](#hyperparameter-tuning)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Results](#results)
- [License](#license)

## Overview

This project applies supervised learning techniques to predict whether a passenger survived the Titanic shipwreck based on features such as age, sex, class, and fare.

## Dataset

The dataset used is the Titanic dataset from [Kaggle](https://www.kaggle.com/c/titanic). It contains information on 891 passengers, including:

- PassengerId
- Survived (Target Variable)
- Pclass
- Name
- Sex
- Age
- SibSp
- Parch
- Ticket
- Fare
- Cabin
- Embarked

## Exploratory Data Analysis (EDA)

Several visualizations were used to understand patterns in the data:

- Count plots by survival status, gender, and passenger class.
- Distribution plots for age and fare.
- Heatmaps for missing values.
- Pairplots to examine feature relationships.

## Data Preprocessing

- Missing values in `Age` were filled using the median age per `Pclass`.
- Dropped columns: `Cabin`, `Ticket`, `Name`, and `PassengerId`.
- Categorical variables (`Sex`, `Embarked`) were encoded using `OrdinalEncoder`.
- Final features used: `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`.

## Modeling

Three classification models were implemented:

- **K-Nearest Neighbors (KNN)**
- **Logistic Regression**
- **Support Vector Machine (SVM)**

Initial results for KNN:
- **Training Accuracy**: ~78%
- **Testing Accuracy**: ~72%

## Hyperparameter Tuning

- The value of `n_neighbors` in KNN was tuned from 1 to 30.
- A loop was used to evaluate each configuration and track accuracy on training and test sets.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Abhilash0209/Machine-learning-.git
   cd titanic-survival-prediction
