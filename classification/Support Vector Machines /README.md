# 🌸 Support Vector Machine (SVM) on Iris Dataset

This project serves as a foundational guide to implementing and analyzing the **Support Vector Machine (SVM)** algorithm. It focuses on the crucial steps of **Exploratory Data Analysis (EDA)**, **Feature Scaling**, and **Hyperparameter Analysis** using the classic and highly separable **Iris dataset**.

---

##  Project Goals
- Demonstrate the **end-to-end pipeline** of a classification project using Scikit-learn.  
- Highlight the critical role of **Feature Scaling** for distance-based algorithms like SVM.  
- Analyze the impact of the **Regularization Parameter `C`** on model accuracy and margin.  
- Visualize **feature relationships** (Pair Plot) and the **Decision Boundary** using PCA.  

---

## Key Results
he model achieved **perfect separation** on the test data when the parameter `C` was optimally set.

### Final Performance Metrics (C = 1.0)

| Metric      | Setosa | Versicolor | Virginica | Accuracy | Macro Avg | Weighted Avg |
|-------------|--------|------------|-----------|----------|------------|---------------|
| Precision   | 1.00   | 1.00       | 1.00      | 1.00     | 1.00       | 1.00          |
| Recall      | 1.00   | 1.00       | 1.00      | 1.00     | 1.00       | 1.00          |
| F1-Score    | 1.00   | 1.00       | 1.00      | 1.00     | 1.00       | 1.00          |
 
## Analysis of Parameter `C`
The parameter **C** controls the regularization in the SVM model, defining the trade-off between maximizing the separation margin and minimizing classification errors.

| Parameter `C` | Accuracy | Model Behavior |
|---------------|----------|----------------|
| **C = 0.1**   | 0.97 (97%) | **Soft Margin:** Wider margin, tolerates some errors for better generalization. |
| **C = 1.0**   | 1.00 (100%) | **Optimal:** Achieves perfect separation on the clean Iris dataset. |


---

## Confusion Matrix
The confusion matrix confirms that **all 30 test samples were classified correctly**:
[[10 0 0]
[ 0 9 0]
[ 0 0 11]]

---

## Visualizations
The notebook includes several key plots to illustrate the data and model behavior:

- **Feature Pair Plot (EDA):** Shows feature interactions. Clear separability of **Setosa**, while Versicolor and Virginica require a more complex boundary.
  [Feature Pair Plot](images/Pair_Plot.png)
- **Correlation Heatmap:** Reveals high correlation between **Petal Length** and **Petal Width**, suggesting feature redundancy.
 [ Correlation Heatmap](images/Feature_Correlation_Heatmap.png)
- **Decision Boundary (PCA):** After dimensionality reduction, the SVM (with RBF Kernel) perfectly separates the three classes in 2D space.  
[Decision Boundary](images/SVM_Decision_Boundary.png)
---

## References
- [Medium - Intuitive Explanation of SVM](https://medium.com/low-code-for-advanced-data-science/support-vector-machines-svm-an-intuitive-explanation-b084d6238106)  
- [GeeksforGeeks - Support Vector Machine Introduction](https://www.geeksforgeeks.org/support-vector-machine-algorithm/)  
- [Scikit-learn - SVM Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)  



