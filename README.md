
# Data Science Seminar Project

This project leverages machine learning models to predict house prices based on features like location, size, amenities, and more. The analysis explores multiple models, evaluates their performance, and provides a user-friendly prediction mechanism for unseen data.



## Table of Contents
1. [Overview](#overview)
2. [Requirements](#requirements)
3. [Dataset](#dataset)
4. [Data Preprocessing](#data-preprocessing)
5. [Models Used](#models-used)
6. [Performance Metrics](#performance-metrics)
7. [Feature Importance](#feature-importance)
8. [Usage](#usage)
9. [Results](#results)
10. [Acknowledgments](#acknowledgments)

---

## Overview

This project uses various machine learning models, including tree-based algorithms and neural networks, to analyze and predict real estate prices. Key highlights include:
- Data preprocessing for handling categorical and numerical data.
- Comparison of models like XGBoost, LightGBM, Random Forest, CatBoost, Gradient Boosting, and Neural Networks.
- Visualization of model performance and feature importance.

---

## Requirements

- Python 3.10+
- Libraries:
  - pandas
  - scikit-learn
  - xgboost
  - tensorflow
  - catboost
  - lightgbm
  - matplotlib
  - seaborn

Install the required libraries using:
pip install -r requirements.txt




## Dataset

- **Source:** Cleaned and preprocessed dataset with real estate features.
- **Columns:** Includes attributes like city, province, latitude, longitude, lease term, type, beds, baths, square footage, Walk Score, and Bike Score.
- **Sample Rows:** Data about various property listings with their features.

---

## Data Preprocessing

- **Steps:**
  1. Dropped unnecessary columns such as `rentfaster_id`, `address`, and `link`.
  2. Handled missing values by dropping rows with NaNs.
  3. Converted categorical values into numerical labels using `LabelEncoder`.
  4. Normalized numerical features using `StandardScaler`.

---

## Models Used

1. **XGBoost Regressor**
2. **CatBoost Regressor**
3. **LightGBM Regressor**
4. **Gradient Boosting Regressor**
5. **Random Forest Regressor**
6. **Neural Network**

---

## Performance Metrics

Each model was evaluated using:
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **R² Score**

### Summary of Model Performance
| Model                | MAE    | MSE      | R²    |
|----------------------|--------|----------|-------|
| XGBoost              | 116.99 | 32744.09 | 0.96  |
| LightGBM             | 129.98 | 41424.17 | 0.95  |
| Gradient Boosting    | 112.45 | 29713.67 | 0.96  |
| Neural Network       | 350.49 | 261372.39| 0.68  |
| Random Forest        | 47.36  | 15719.71 | 0.98  |
| CatBoost             | 79.37  | 17973.28 | 0.98  |

---

## Feature Importance

The importance of features was analyzed using each model's specific importance calculation. Below is a comparison of the relative feature importance:

- Top Features Across Models:
  - **Square Footage**
  - **Number of Bathrooms**
  - **Walk Score**
  - **Bike Score**

### Visualization
Feature importance charts were generated for better insights into how each feature contributes to the predictions.

---

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/data-science-seminar-project.git
   ```
2. Navigate to the project directory:
   ```bash
   cd data-science-seminar-project
   ```
3. Run the Jupyter Notebook or Python scripts to preprocess data, train models, and make predictions.

---

## Results

- **Best-performing model:** Random Forest Regressor
- **Example prediction:**
  - Input: 2 beds, 2 baths, 980 sq. ft., Walk Score: 24
  - Predicted Price: **$2141.53**

---

## Acknowledgments

Special thanks to the contributors and the dataset providers for enabling this project.
```
