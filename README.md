# Quantum Support Vector Regression (QSVR) for Solar Radiation Prediction

This project implements a Quantum Support Vector Regression (QSVR) model to predict solar radiation based on various meteorological features using PennyLane and TensorFlow. The model leverages quantum kernel methods to enhance prediction accuracy.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Evaluation Metrics](#evaluation-metrics)
- [License](#license)

## Introduction

Solar radiation prediction is crucial for various applications, including solar energy generation and climate modeling. This project uses quantum computing techniques to predict solar radiation based on features such as temperature, pressure, wind speed, the day of the year, and hour of the day.

## Installation

To run this project, you will need to have Python 3.x installed along with the following packages:

- `pennylane`
- `tensorflow`
- `numpy`
- `scikit-learn`

You can install the necessary packages using pip:

```bash
pip install pennylane tensorflow numpy scikit-learn

'''

## Usage

Load Your Dataset: Ensure you have a dataset named solarprediction.csv containing the relevant features.
Run the Script: Execute the script that implements the QSVR model. This script standardizes the data, computes the quantum kernel, and fits the model.
Evaluate the Model: After training, the script will output evaluation metrics, including Mean Squared Error (MSE), Mean Absolute Error (MAE), and R² Score.

##Data

The dataset should be in a CSV file named solarprediction.csv and contain the following features:

Temperature: Ambient temperature in degrees Celsius.
Pressure: Atmospheric pressure in hPa.
Speed: Wind speed in m/s.
Day: Day of the year (1-365).
Hour: Hour of the day (0-23).
Radiation: Target variable representing solar radiation in watts per square meter (W/m²).
Ensure that the dataset is preprocessed and ready for training.

##Evaluation Metrics

The model performance is evaluated using the following metrics:

Mean Squared Error (MSE): Measures the average squared difference between actual and predicted values.
Mean Absolute Error (MAE): Measures the average absolute difference between predicted and actual values.
R² Score: Represents the proportion of variance explained by the model.
