# Sensor Calibration for O3 and NO2 in Indian Conditions

## Project Overview

This project focuses on calibrating Ozone (O3) and Nitrogen Dioxide (NO2) sensors to accurately measure the true levels of these pollutants under Indian environmental conditions. Given the complexity and variability in pollutant levels, the project explores various linear and non-linear models to achieve the best calibration with minimal error.

## Problem Statement

[Include a summary or attach the problem statement here.]

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

## Installation and Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sensor-calibration.git
Navigate to the project directory:

bash
Copy code
cd sensor-calibration
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Run the model training script:

bash
Copy code
python train_model.py
Evaluate the models and view results:

bash
Copy code
python evaluate_model.py
Files and Directory Structure
train_model.py: Script to train the models.
evaluate_model.py: Script to evaluate model performance.
data/: Directory containing the dataset.
models/: Directory where trained models are saved.
README.md: Project overview and instructions.
requirements.txt: Required Python libraries.
Conclusion
This project successfully identifies the most suitable linear and non-linear models for sensor calibration under Indian environmental conditions. The linear regression and KNN models stood out due to their low error rates and manageable model sizes, making them ideal for practical applications.

Future Work
Explore more advanced models and feature engineering techniques.
Extend the calibration approach to other pollutants and geographical regions.
Implement the models in real-time sensor applications to test their performance in the field.
