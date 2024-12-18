# Regression and Classification Project

This project focuses on solving both regression and classification problems using various machine learning models. It includes data preprocessing, model development, hyperparameter tuning, and performance comparison for multiple algorithms.

---

## Dataset Information

The datasets used in this project were obtained as open-source data from the internet. They have been uploaded to GitHub and can be accessed via the following links:

- [Rain in Australia](https://github.com/AysenurYrr/ML-Lab/tree/main/Rain%20in%20Australia)
- [UCI Air Quality](https://github.com/AysenurYrr/ML-Lab/tree/main/UCI%20Air%20Quality)

### Key Notes
- Exploratory Data Analysis (EDA) has already been performed in prior projects and is not included in this notebook.
- The datasets contain features relevant to regression and classification tasks, with both numerical and categorical variables.

### Data Sources
1. **Rain in Australia**:
   - Contains weather data from Australian regions.
   - Suitable for classification tasks, such as predicting whether it will rain tomorrow based on weather patterns.

2. **UCI Air Quality**:
   - Includes air quality measurements with time-series data.
   - Useful for regression tasks, like predicting pollutant levels based on sensor readings.

### Preprocessing Steps
- Missing values in categorical and numerical features were handled using imputation techniques:
  - Modes for categorical features (region-specific).
  - Means or medians for numerical features (location-based or global averages).
- Rows with excessive missing data or missing target values were removed.
- Features were scaled using MinMax Scaler for consistency.
- For the classification task, the dataset was balanced using SMOTE to address class imbalance.

---

## Project Structure

### 1. Regression Problem
#### A. Data Preprocessing
- Dropping null values
- Handling missing values in features and target
- Scaling features using MinMax Scaler
- Train-test split with a time-series approach to maintain temporal order

#### B. Modelling
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost
- Custom functions for:
  - Model training and evaluation
  - Hyperparameter tuning
  - Feature importance analysis
  - Model interpretability

#### C. Comparison
- Models are compared based on performance metrics like Mean Squared Error (MSE) and R².

---

### 2. Classification Problem
#### A. Data Preprocessing
- Handling categorical and numerical missing values
- Encoding categorical features and scaling numerical features
- Train-test splitting and balancing the dataset using SMOTE

#### B. Modelling
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier
- Custom functions for:
  - Model training and evaluation
  - Hyperparameter tuning
  - Extracting and analyzing the top 10 important features

#### C. Comparison
- Models are evaluated and compared based on metrics like Accuracy, F1-Score, Precision, and Recall.

---

## Key Features
- **Custom Utility Functions**: Simplify tasks like hyperparameter tuning, feature importance extraction, and model evaluation.
- **Hyperparameter Tuning**: Utilizes GridSearchCV for optimal parameter selection.
- **Feature Importance Analysis**: Includes methods like SHAP (SHapley Additive exPlanations) for interpretability.
- **Balanced Data Training**: Uses techniques like SMOTE to address class imbalance in the classification problem.
- **Model Comparison**: Comprehensive evaluation of models to determine the best-performing algorithms for both tasks.

---

## Getting Started

### Requirements
- Python 3.8 or higher
- Libraries:
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `xgboost`
  - `matplotlib`
  - `seaborn`
  - `imblearn`

### Instructions
1. Clone the repository.
2. Install the required Python libraries.
3. Run the notebook file to execute the regression and classification tasks.

---

## Results
- **Regression Models**: Evaluated based on MSE and R².
- **Classification Models**: Evaluated on Accuracy, F1-Score, Precision, and Recall.
- Feature importance analysis highlights the key predictors for each problem.

