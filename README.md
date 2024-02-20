# Battery State of Charge (SOC) Prediction

This repository contains code for predicting the State of Charge (SOC) of a battery using various machine learning models.

## Data

The dataset consists of battery data collected at a temperature of 25 degrees Celsius, including:

- DST (Dynamic Stress Test) data
- FUDS (Federal Urban Driving Schedule) data

## Features

The following features are used for prediction:

- Temperature(degree_C)
- Current(A)
- Voltage(V)
- Discharge_Capacity - Charge_Capacity(Ah)
- Discharge_Energy - Charge_Energy(Wh)
- dV/dt(V/s)

## Models

The following models are explored:

- Linear Regression
- Random Forest Regressor
- XGBoost Regressor
- Neural Network (TensorFlow Keras)

## Evaluation

Model performance is evaluated using Mean Squared Error (MSE).

## Usage

1. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn sklearn xgboost shap tensorflow
   Run the main.py script (or the respective model scripts).
## Additional Information

- The code includes data preprocessing, feature engineering, model training, evaluation, and feature importance analysis.
- SHAP (SHapley Additive exPlanations) is used to explain feature importance for the XGBoost model.
- Correlation matrices are visualized to explore relationships between features.
- Learning curves are plotted to visualize model training progress.
  
## Project Structure
- BMS_Final.ipynb : Main script to run all model training and evaluation steps.
- data/: Directory containing the dataset files (dst25.xlsx and fuds25.xlsx).
