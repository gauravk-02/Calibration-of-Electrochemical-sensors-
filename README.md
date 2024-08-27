# Sensor Calibration for O3 and NO2 in Indian Conditions

## Project Overview

This project focuses on calibrating Ozone (O3) and Nitrogen Dioxide (NO2) sensors to accurately measure the true levels of these pollutants under Indian environmental conditions. Given the complexity and variability in pollutant levels, the project explores various linear and non-linear models to achieve the best calibration with minimal error.

## Approach

1. **Model Implementation:**
    - Explored both linear and non-linear models including:
        - **Linear Models:**
            - Ridge Regression
            - Lasso Regression
        - **Non-Linear Models:**
            - Random Forest
            - Decision Tree
            - K-Nearest Neighbor (KNN)
    - Implemented different models to understand their performance under varying conditions.

2. **Hyperparameter Tuning:**
    - For Ridge and Lasso regression, varied the regularization parameter α to minimize the Mean Absolute Error (MAE).
    - For the KNN model, varied the number of neighbors (n) to find the optimal point that decreases MAE.

3. **Model Evaluation:**
    - Checked for overfitting and underfitting in each model.
    - Adjusted models accordingly to reduce error and improve performance.
    - Compared models based on MAE and model size to identify the best-performing ones.

## Results

- **Best Linear Model:** Linear Regression with the least Mean Absolute Error (MAE) and minimal model size.
- **Best Non-Linear Model:** K-Nearest Neighbor (KNN), providing a good balance between accuracy and complexity.

