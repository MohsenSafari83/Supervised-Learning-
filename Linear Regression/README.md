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

## What You Will Learn
1. **Linear Regression Theory**
   - How the model fits a line to predict target values.
   - Concepts of **training error**, **test error**, and **RMSE**.
2. **Polynomial Regression (Optional Extension)**
   - How to extend linear regression to higher-degree features.
3. **Regularization Techniques**
   - Ridge Regression (L2) and Lasso Regression (L1) for reducing overfitting.
4. **Visualization**
   - Plotting predicted vs actual values.
   - RMSE curves for different polynomial degrees and regularization parameters.

---
# Linear Regression Results

### Multivariate Linear Regression (MLR)
The plot below shows predicted vs actual house values using **MLR**:

![MLR Prediction](images/mlr.png)

### Polynomial Linear Regression (PLR)
The plot below shows predicted vs actual house values using **PLR** (degree 2):

![PLR Prediction](images/plr.png)

