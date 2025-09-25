#  Data Preprocessing  

Data preprocessing is an essential step in any Machine Learning workflow.  
The quality of your data directly affects the performance of your model.  

This repository contains notebooks and explanations about different **data preprocessing techniques** and how to implement them in Python (using pandas, NumPy, scikit-learn, seaborn, matplotlib).  

---

## 🔹 Topics Covered  

### 1. Handling Missing Data  
- Sources of missing values  
- Techniques:  
  - `fillna()`  
  - `dropna()`  
  - Scikit-learn’s `SimpleImputer`  

---

### 2. Handling Categorical Variables  
- **One-Hot Encoding** with pandas `get_dummies`  
- **Label Encoding** with scikit-learn  
- Using `ColumnTransformer` for preprocessing pipelines  

---

### 3. Feature Scaling  
- Why scaling matters (especially for distance-based algorithms like KNN, SVM)  
- **Normalization (Min-Max Scaling)**  
- **Standardization (Z-score Scaling)**  
- When to use Normalization vs Standardization  

---

### 4. Distance-Based Algorithms  
- Why scaling is critical for algorithms based on Euclidean distance  
- Examples with K-Nearest Neighbors (KNN)  

---

### 5. Model Evaluation (Cross-Validation)  
- **k-fold cross-validation**  
- **Stratified k-fold cross-validation**  
- Choosing the right strategy depending on dataset balance  

---

### 6. Data Analysis Tools  
- **Correlation Matrix** and heatmaps for feature relationships  
- Outlier detection:  
  - **Z-score Method**  
  - **IQR Method**  

---

### 7. Feature Engineering  
- **Feature Selection**:  
  - Filter methods (SelectKBest)  
  - Wrapper methods (Forward/Backward Selection)  
  - Embedded methods (Lasso, Ridge, Tree-based)  
- **Dimensionality Reduction**:  
  - Introduction to PCA (Principal Component Analysis)  
  - Why and when to reduce dimensions  

---

### 8. Data Transformation  
- Making data more normally distributed  
- Techniques:  
  - Log Transformation  
  - Square Root Transformation  
  - Reciprocal Transformation  
  - Box-Cox Transformation  
  - Yeo-Johnson Transformation  

---
## 9. Dimensionality Reduction (PCA)  
- Reduces the number of features while retaining the most important information.  
- Helps avoid **curse of dimensionality**, reduces overfitting, and improves computation efficiency.  
- Example: PCA can compress a dataset with 100 features into 10–20 important ones.  

---

## 10. Train-Test Split  
- Always split your dataset into **training** and **testing** sets.  
- Training set → used to train the model.  
- Testing set → used to evaluate performance on unseen data.  
- Typically, **70/30 or 80/20 splits** are common.  
- Alternatively, use **cross-validation** for more robust evaluation.  

---

## 11.  Why Use Pipelines in Scikit-learn?  
When building machine learning models, preprocessing steps like **handling missing values, encoding categorical variables, scaling, and dimensionality reduction** must be done **before** training.  

❌ If you apply preprocessing separately to train and test data, you risk:  
- Data leakage  
- Inconsistent transformations  

✅ Pipelines ensure that the **same transformations** are applied to both training and testing data in the correct order.  

---
Clone the repository:  
```bash
git clone https://github.com/your-username/Preprocessing-data.git
cd Preprocessing-data

