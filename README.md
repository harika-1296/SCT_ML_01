# SCT_ML_01
Predicting house prices using Multiple Linear Regression based on square footage, bedrooms, and bathrooms.
# House Price Prediction using Multiple Linear Regression

## Overview

This project implements a Multiple Linear Regression model to predict house prices based on important property features such as:

* Square Footage
* Number of Bedrooms
* Number of Bathrooms

The model learns the relationship between these features and house prices using historical housing data and predicts prices for unseen properties.

---

## Problem Statement

House prices are influenced by several factors, including property size and amenities. The objective of this project is to build a machine learning model capable of estimating house prices accurately using Multiple Linear Regression.

---

## Dataset

The dataset contains the following features:

| Feature        | Description                            |
| -------------- | -------------------------------------- |
| Square_Footage | Total area of the house in square feet |
| Bedrooms       | Number of bedrooms                     |
| Bathrooms      | Number of bathrooms                    |
| Price          | Target variable (House Price)          |

Dataset file:
`HousePricePrediction.xlsx`

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* OpenPyXL

---

## Project Workflow

### 1. Data Collection

* Loaded housing dataset from Excel file.

### 2. Data Preprocessing

* Checked for missing values.
* Selected relevant features.
* Prepared data for model training.

### 3. Exploratory Data Analysis (EDA)

* Analyzed relationships between features and target variable.
* Visualized distributions and trends.

### 4. Model Building

* Split data into training and testing sets.
* Trained Multiple Linear Regression model.

### 5. Model Evaluation

Evaluated performance using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

### 6. Prediction

Generated house price predictions for test data and new input values.

---

## Model Training

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()
model.fit(X_train, y_train)
```

---

## Evaluation Metrics

```python
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
```

Metrics used:

* MAE
* MSE
* RMSE
* R² Score

---

## Visualization

Actual vs Predicted House Prices visualization was generated to evaluate model performance.

Example:

* Actual Prices on X-axis
* Predicted Prices on Y-axis

---

## Results

The model successfully learned the relationship between:

* House Size
* Bedrooms
* Bathrooms

and produced house price predictions with satisfactory accuracy.

---

## Future Improvements

* Add more housing features such as:

  * Location
  * Age of Property
  * Garage Availability
  * Nearby Facilities

* Experiment with:

  * Random Forest Regressor
  * XGBoost Regressor
  * Gradient Boosting Regressor

* Deploy using:

  * Streamlit
  * Flask
  * FastAPI

---

## Project Structure

```text
House-Price-Prediction/
│
├── data/
├── notebooks/
├── src/
├── outputs/
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Author

Harika Reddy Gundla

Machine Learning Enthusiast | Data Science Learner

---

## License

This project is licensed under the MIT License.
