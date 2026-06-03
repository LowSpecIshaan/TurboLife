# TurboLife – Remaining Useful Life Prediction for Turbofan Engines

TurboLife is a deep learning-based predictive maintenance system that estimates the **Remaining Useful Life (RUL)** of turbofan engines using multivariate sensor time-series data. The project leverages Long Short-Term Memory (LSTM) networks to model engine degradation patterns and predict the number of operational cycles remaining before failure.

## Overview

Predictive maintenance is a critical application of machine learning in the aerospace industry. By analyzing engine sensor readings over time, TurboLife forecasts engine health and helps identify potential failures before they occur.

The project includes:

* Data preprocessing and sequence generation
* LSTM-based RUL prediction
* Model evaluation using regression metrics
* Interactive Gradio dashboard for real-time predictions

## Features

* Multivariate time-series forecasting using LSTM networks
* Rolling-window sequence generation pipeline
* Engine health assessment based on predicted RUL
* Interactive web interface built with Gradio
* Model checkpointing and performance visualization

## Tech Stack

* Python
* TensorFlow / Keras
* NumPy
* Pandas
* Matplotlib
* Gradio

## Model Architecture

* Stacked LSTM layers
* Dropout regularization
* Dense output layer for RUL regression
* Early stopping and model checkpointing

## Results

| Metric                         | Value |
| ------------------------------ | ----- |
| Mean Absolute Error (MAE)      | 46.9  |
| Root Mean Squared Error (RMSE) | 55.7  |

The model successfully learns temporal degradation patterns and produces reliable Remaining Useful Life estimates on unseen engine data.

## Project Structure

```text
TurboLife/
│
├── rul.ipynb                  # Training and evaluation notebook
├── best_rul_model.keras       # Best saved model
├── rul_predictor.keras        # Final trained model
└── README.md
```

## Future Improvements

* Training on NASA CMAPSS benchmark datasets
* Hyperparameter optimization
* Transformer-based time-series models
* Explainable AI techniques for maintenance decisions
* Deployment as a cloud-hosted application
