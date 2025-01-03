# FUTURE_ML_01
# Predicting House Prices Using Linear Regression

This repository contains a project that implements a **Linear Regression Model** to predict house prices based on specific features, including square footage, the number of bedrooms, and bathrooms. The project is part of a hands-on data science exercise aimed at understanding the end-to-end process of building and evaluating predictive models.

## Project Overview

The goal of this project is to predict house prices using structured data and apply essential data preprocessing techniques, feature engineering, and model evaluation steps. The dataset includes various house attributes, and the analysis focuses on simplifying the prediction task by selecting relevant features.

### Key Features Used:
- **GrLivArea**: Above ground living area (square footage).
- **BedroomAbvGr**: Number of bedrooms above ground.
- **FullBath**: Number of full bathrooms above ground.
- **Optional**: TotalBathrooms (calculated feature incorporating all bathrooms).

## Workflow Description

The notebook follows these steps:
1. **Data Loading**:
   - Training and testing datasets are loaded into the notebook.

2. **Exploratory Data Analysis (EDA)**:
   - Key features and their distributions are visualized to understand the data.
   - Relationships between selected features and the target variable (`SalePrice`) are analyzed.

3. **Data Cleaning and Preprocessing**:
   - Missing values are handled appropriately.
   - Categorical variables are encoded using **Scikit-learn's OneHotEncoder** to ensure consistent representation.
   - A calculated feature, `TotalBathrooms`, is introduced for better prediction accuracy (if included).

4. **Feature Selection**:
   - Relevant features (`GrLivArea`, `BedroomAbvGr`, `FullBath`) are selected for simplicity.
   - Optionally, additional features (e.g., `TotalBathrooms`) are engineered and included.

5. **Model Implementation**:
   - A **Linear Regression Model** is built using Scikit-learn.
   - The model is trained on the training set and evaluated on a validation set using metrics like:
     - **Mean Squared Error (MSE)**
     - **\( R^2 \)-Score**
   - Cross-validation is performed for additional performance insights.

6. **Prediction**:
   - Predictions are made on the test dataset using the trained model.
   - The predictions are saved as a CSV file for further evaluation or submission.


## How to Run the Notebook

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/predict-house-prices.git
   cd predict-house-prices
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt

3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Task_01_Predict_House_Prices.ipynb

4. Follow the steps in the notebook to explore the data, preprocess it, train the model, and make predictions.

## Outputs

- **Validation Metrics:** Mean Squared Error and \( R^2 \)-Score are calculated on the validation set.
 **Predictions File:** A CSV file (`house_price_predictions.csv`) containing predictions for the test dataset is generated.

## Dataset
The datasets used in this project are provided by the [Kaggle competition House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques).


## Author
This project was created as part of a machine learning learning initiative. Contributions, suggestions, or feedback are welcome!
