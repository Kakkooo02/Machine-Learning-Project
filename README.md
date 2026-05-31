# Used Car Price Prediction

This project uses data science and machine learning techniques to predict used car prices based on vehicle specifications, categorical features, and listing information.

The project was developed in Python using Jupyter Notebook. It includes data cleaning, preprocessing, feature engineering, model training, model saving, and testing on unseen data.

## Overview

Used car prices depend on many factors, including model, year, mileage, engine specifications, location, fuel type, transmission type, and other vehicle features. The goal of this project is to build a regression model that can estimate the value of a used car based on available data.

The project follows a complete machine learning workflow:

1. Load and inspect the dataset
2. Clean irrelevant and missing values
3. Preprocess numerical and categorical features
4. Apply feature engineering
5. Train a neural network regression model
6. Save preprocessing objects and the trained model
7. Test the model on unseen data
8. Evaluate prediction performance

## Features

* Data cleaning and column filtering
* Missing value handling
* Numerical feature scaling
* Categorical feature encoding
* Feature engineering
* Neural network regression model
* Model evaluation on unseen data
* Saved preprocessing pipeline components
* Actual vs predicted price comparison

## Tech Stack

| Area                 | Tools                      |
| -------------------- | -------------------------- |
| Language             | Python                     |
| Notebook environment | Jupyter Notebook           |
| Data handling        | Pandas, NumPy              |
| Preprocessing        | Scikit-learn               |
| Machine learning     | TensorFlow, Keras          |
| Model type           | Neural network regression  |
| Model persistence    | Pickle, Keras model saving |


## Project Workflow

### 1. Data Loading

The dataset is loaded using Pandas and inspected to understand the available vehicle-related features.

### 2. Data Cleaning

The cleaning stage removes irrelevant, repeated, or unnecessary columns. Missing values are handled depending on the type and importance of each feature.

### 3. Feature Preprocessing

The project separates features into numerical and categorical columns.

Numerical features are processed using imputation and scaling, while categorical features are encoded using one-hot encoding.

### 4. Feature Engineering

Additional feature transformations are applied to improve model performance. Some high-cardinality categorical values are grouped, and selected encoded features are merged or removed when needed.

### 5. Model Training

A neural network regression model is trained to predict used car prices. The model uses dense layers and dropout layers to learn relationships between car features and price.

### 6. Model Testing

The trained model is tested on unseen car data. The testing notebook loads the saved model and preprocessing objects, applies the same preprocessing steps to the unseen dataset, and compares predicted values with actual values.

## Model Summary

The final neural network model includes multiple dense layers with dropout regularization. The model is designed for regression, where the output is a predicted used car price.

## Results

The model was evaluated on unseen data using Mean Absolute Error.

```text
Mean Absolute Error on test data: approximately 133,291
```

The testing notebook also compares actual and predicted prices for sample vehicles to evaluate how close the model predictions are to real values.

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/Kakkooo02/Machine-Learning-Project.git
cd DataSci
```

2. Install the required packages:

```bash
pip install -r requirements.txt
```

3. Open the main notebook:

```text
used_car_price_prediction.ipynb
```

4. Run the notebook cells in order.

5. To test the saved model on unseen data, open:

```text
model_testing_unseen_data.ipynb
```

## Notes

Some files used during training and testing may need to be included locally, such as:

```text
cars_unseen_data.csv
trained_model.keras
scaler.pkl
one_hot_encoder.pkl
imputer.pkl
```

If these files are not uploaded to GitHub, they should be listed in the project report or shared separately when needed.

## What I Learned

Through this project, I practiced:

* Cleaning real-world vehicle data
* Handling missing and inconsistent values
* Preparing numerical and categorical features
* Using one-hot encoding and scaling
* Building a neural network regression model
* Testing machine learning models on unseen data
* Evaluating predictions using Mean Absolute Error

## Future Improvements

* Improve feature selection
* Tune neural network architecture
* Compare the neural network against models such as Random Forest, XGBoost, or Linear Regression
* Add more visualizations for model performance
* Use cross-validation

## Author

Created by Kakkooo0
