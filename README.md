# Regression with a Flood Prediction

This repository contains code for the Kaggle competition where the goal is to predict the probability of floods based on various climatic factors. This is a regression problem statement, and we use various machine learning models to tackle it.

## Table of Contents
- [Overview](#overview)
- [Data](#data)
- [Installation](#installation)
- [Usage](#usage)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Contributing](#contributing)
- [License](#license)

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

## Usage

To run the code, follow these steps:

1. **Prepare the Data**: Ensure that your data is in the `data` directory. You may need to adjust the paths in the code accordingly.

2. **Preprocess the Data**: Run the preprocessing script to clean and prepare the data for training.

    ```bash
    python scripts/preprocess.py
    ```

3. **Train the Model**: Use the training script to train the machine learning models. For example, to train an XGBoost model, run:

    ```bash
    python scripts/train.py --model xgboost --params params/xgboost_params.json
    ```

4. **Evaluate the Model**: After training, evaluate the model on the test set to see its performance.

    ```bash
    python scripts/evaluate.py --model xgboost
    ```

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

```bash
python scripts/train.py --model lightgbm --params params/lightgbm_params.json
```

## Evaluation

The models are evaluated using the R² score to measure the goodness of fit. The evaluation script will output the R² score for the training and test sets.

Example command:

```bash
python scripts/evaluate.py --model lightgbm
```

## Contributing

Contributions are welcome! Please read the [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to contribute to this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to modify the paths and script names to match your actual project structure. This README should give a clear overview of the project and instructions on how to set it up and run it.
