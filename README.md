# Regression with a Flood Prediction

This repository contains code for the Kaggle competition where the goal is to predict the probability of floods based on various climatic factors. This is a regression problem statement, and we use various machine learning models to tackle it.

## Table of Contents
- [Overview](#overview)
- [Data](#data)
- [Installation](#installation)
- [Notebook Intro](#notebook-intro)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Contributing](#contributing)

## Overview

Flooding is a critical issue affecting many regions around the world. Predicting the probability of floods based on climatic factors can help disaster preparedness and management. This project involves building regression models to predict flood probabilities using various climatic features.

## Data

The dataset includes various climatic factors which are listed below. 
- MonsoonIntensity
- TopographyDrainage
- RiverManagement
- Deforestation
- Urbanization
- ClimateChange
- DamsQuality
- Siltation
- AgriculturalPractices
- Encroachments
- IneffectiveDisasterPreparedness
- DrainageSystems
- CoastalVulnerability
- Landslides
- Watersheds
- DeterioratingInfrastructure
- PopulationScore
- WetlandLoss
- InadequatePlanning
- PoliticalFactors
- FloodProbability [Target Variable]

## Installation

To get started with this project, clone the repository and install the required dependencies:

```bash
git clone https://github.com/your-username/flood-prediction.git
cd flood-prediction
pip install -r requirements.txt
```

## Notebook Intro
In the notebook, I will write down the steps I have did in a clear way.
- <b>Import Data</b> - Imported train, test and original data of flood factors.
- <b>Statistics</b> - Understanding the basic descriptive statistics of the data to get the basic idea.
- <b>Exploratory Data Analysis</b> - Done EDA to understand the distributions and relationship between features and target variable.
- <b>Feature Engineering</b> - Created new features that has a linear relationship with the target variable.
- <b>Model Training</b> - Trained all the regression models to understand how each model performs on this type of data.
- <b>Cross Validation</b> - Done Cross Validation to understand whether the model performs consistent across all the folds.
- <b>Prediction</b> - Prediction on test data to submit to competetion

## Model Training

We have used various machine learning models for this task, including:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- AdaBoost Regressor
- LightGBM
- XGBoost
- CatBoost

Each model can be trained by specifying the model name and parameter file. For example, to train a LightGBM model, use:


## Evaluation

The models are evaluated using the R² score to measure the goodness of fit. The evaluation script will output the R² score for the training and test sets.


## Contributing

Contributions are welcome! Please reach out to me if there are any improvements we can do or incase of any doubts at aknandam30@gmail.com


