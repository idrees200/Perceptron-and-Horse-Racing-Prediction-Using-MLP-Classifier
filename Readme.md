# Perceptron and Horse Racing Prediction Using MLP Classifier

## Overview

This repository contains two main parts:

1. **Perceptron Implementation**: A simple implementation of a perceptron to simulate the logic gates AND and OR.
2. **Horse Racing Prediction**: Using a Multi-Layer Perceptron (MLP) classifier to predict the outcome of horse races.

## Part 1: Perceptron Implementation

### Perceptron Class

The `Perceptron` class is implemented with methods to initialize weights and bias, and to predict outputs based on inputs.

### Logic Gates Simulation

- **AND Gate**: 
  - Weights: [0.5, 0.5]
  - Bias: -0.8

- **OR Gate**: 
  - Weights: [0.5, 0.5]
  - Bias: -0.3


## Part 2: Horse Racing Prediction

This section details the steps to predict horse racing outcomes using a Multi-Layer Perceptron (MLP) classifier. The dataset contains various features related to horse racing events, and the goal is to predict whether a horse finishes first in a race.

### Steps Involved

1. **Load Data**: Load the horse racing data from a CSV file into a DataFrame.

2. **Handle Missing Values**: Drop rows with missing values to ensure a clean dataset for training.

3. **Encode Target Variable**: Convert the `calc_position` column to binary values (1 if the horse finished first, 0 otherwise).

4. **Impute Missing Values**: Apply mean imputation to handle any remaining missing values, ensuring all columns have valid numerical entries.

5. **Visualize Data**: Generate visualizations to understand the statistical properties of the dataset, such as distributions and summary statistics.

6. **One-Hot Encoding**:
    - Encode the `race_id` and `horse_id` columns to convert categorical data into numerical format suitable for the model.
    - Create new columns for each unique value in the `race_id` and `horse_id` columns.

7. **Feature Scaling**: Standardize the feature values using a scaler to improve model performance and ensure that all features contribute equally to the model training.

8. **Train-Test Split**: Split the dataset into training and testing sets to evaluate the model's performance and ensure it generalizes well to new data.

9. **MLP Classifier**:
    - Train a Multi-Layer Perceptron classifier on the training data using specified hyperparameters such as the number of hidden layers and activation functions.
    - Evaluate the model by predicting outcomes on the test data and calculating the accuracy.

10. **Evaluate Results**: Print the accuracy of the MLP classifier to assess the model's performance in predicting horse racing outcomes.

### Key Points

- **Data Preparation**: Ensuring the dataset is clean and all variables are in a suitable format for model training is crucial for achieving good predictive performance.
- **Feature Engineering**: One-hot encoding and feature scaling are essential steps to handle categorical data and standardize feature values, respectively.
- **Model Training and Evaluation**: Splitting the data into training and testing sets allows for proper evaluation of the model's generalization capability, while the choice of classifier and its hyperparameters can significantly impact performance.
