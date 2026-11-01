# NASA Turbofan Engine Remaining Useful Life (RUL) Prediction

## Project Overview

This project focuses on predicting the **Remaining Useful Life (RUL)** of aircraft turbofan engines using machine learning.

Remaining Useful Life estimates how many operational cycles an engine can continue running before it reaches a failure condition. Predicting RUL can support predictive maintenance and reduce unexpected equipment failures.

## Dataset

- **Dataset:** NASA C-MAPSS (Commercial Modular Aero-Propulsion System Simulation)
- **Subset:** FD001
- **Data type:** Simulated turbofan engine sensor data
- **Features:** Engine operating settings and sensor measurements

The dataset is not included in this repository. It can be obtained from the [NASA Open Data Portal](https://data.nasa.gov/dataset/cmapss-jet-engine-simulated-data).

## Project Workflow

1. Data loading and exploration
2. Exploratory Data Analysis (EDA)
3. Sensor correlation and trend analysis
4. Remaining Useful Life (RUL) label generation
5. Feature preparation and preprocessing
6. Training and evaluating machine learning models
7. Model comparison and performance analysis

## Machine Learning Algorithms

The notebook explores the following regression models:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- Voting Regressor
- Stacking Regressor

A Dummy Regressor is also used as a baseline.

## Model Evaluation

The models are evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Validation Results

| Model | MAE | RMSE |
|---|---:|---:|
| Random Forest | 25.754 | 35.287 |
| Stacking | 26.213 | 35.219 |
| Gradient Boosting | 26.366 | 35.629 |
| Voting | 26.826 | 35.952 |
| Decision Tree | 29.282 | 39.891 |
| Linear Regression | 30.111 | 38.133 |

### Official Test Set Results

Random Forest Regressor:

- MAE: 24.30
- RMSE: 32.97
- R² Score: 0.3705

## Further Analysis

The notebook also includes:

- Feature importance analysis
- Residual analysis
- Learning curves
- Sensor trend visualizations
- Model performance comparison

## Tools and Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Repository Contents

- `Supervised_learning_Case_Study_organized.ipynb` — Main notebook containing data analysis, model training, evaluation, and visualizations.
- `README.md` — Project documentation.

## Note

This project is an experimental machine learning study using simulated engine degradation data. The reported metrics describe the experiments conducted in the notebook.
