# Linear Regression on California Housing Dataset

## Overview
This project demonstrates the use of **Linear Regression** on the **California Housing dataset**. The goal is to predict **median house values** based on features such as median income, average rooms, population, etc.

The project includes both **theoretical explanations** and **practical implementation** in Python.

---

## Dataset 
Each record represents a **census block group** in California with the following features:

| Feature     | Description |
|-------------|-------------|
| **MedInc**  | Median income of block residents (in tens of thousands of dollars). |
| **HouseAge**| Median age of houses in the block. |
| **AveRooms**| Average number of rooms per house. |
| **AveBedrms** | Average number of bedrooms per house. |
| **Population** | Block population. |
| **AveOccup** | Average household size (occupants per house). |
| **Latitude** | Block latitude. |
| **Longitude** | Block longitude. |
| **MedHouseVal** | **Target**: Median house value (in hundreds of thousands of dollars). |


---


## Methodology & Steps
### 1. Data Loading & Cleaning
- Load the California Housing dataset (via `sklearn.datasets.fetch_california_housing`).  
- Check for missing values and handle appropriately.  

### 2. Data Preprocessing
- **Split dataset** into training and testing sets.  
- **Feature scaling** using `StandardScaler` or `MinMaxScaler` to normalize input features, improving regression performance.  

### 3. Model Implementation
- Train a **Linear Regression model** (`sklearn.linear_model.LinearRegression`) on the training set.  
- Extract model coefficients (`coef_`) to analyze the impact of each feature.  

### 4. Model Evaluation
- Make predictions on the test set.  
- Calculate performance metrics:  
  - **MAE** (Mean Absolute Error)  
  - **MSE / RMSE** (Mean Squared Error / Root Mean Squared Error)  
  - **R² Score** (explained variance of the target variable)  

---
# Linear Regression Results

### Multivariate Linear Regression (MLR)
The plot below shows predicted vs actual house values using **MLR**:

![MLR Prediction](images/mlr.png)

### Polynomial Linear Regression (PLR)
The plot below shows predicted vs actual house values using **PLR** (degree 2):

![PLR Prediction](images/plr.png)

