# Ensemble Learning: Machine Learning Ensemble Methods

## Introduction and Project Goal
This repository is dedicated to the in-depth theoretical concepts and implementation of advanced **Ensemble Learning methods** in Machine Learning. Ensemble learning significantly boosts model performance by intelligently combining the outputs of multiple base models (weak learners) to achieve higher accuracy and stability than any single model alone.

| Key Concept | Bagging | Boosting |
|------------|---------|---------|
| **Primary Goal** | Reduces Variance | Reduces Bias |
| **Training Method** | Parallel and Independent | Sequential and Dependent |

---

## Table of Contents and Concepts Covered

The content of this documentation is structured around the main categories of ensemble learning techniques:

### 1. Parallel Methods
- Trained in parallel to reduce **Variance** and prevent **Overfitting** in strong, unstable base models.

#### Bagging (Bootstrap Aggregating)
- Uses **Bootstrap Resampling** (sampling with replacement).  
- Aggregates results via **Majority Voting** (classification) or **Averaging** (regression).

#### Random Forest
- Uses **Decision Trees** as base models.  
- Applies **Random Feature Subspace Selection** at each node (Feature Randomness) to decorrelate the trees.

---

### 2. Sequential Methods
- Trained sequentially, with each new model focusing on correcting errors of preceding models.  
- Main goal: Reduce **Bias** and improve predictive capability.

#### Boosting
- Implements **variable sample weighting** based on classification difficulty.  
- Utilizes **Weak Learners** (e.g., shallow Decision Trees or Stumps).

##### AdaBoost (Adaptive Boosting)
- Updates sample weights and calculates the final model weight (αₘ) based on the weighted error (ϵₘ).

##### Gradient Boosting
- Minimizes error using **Gradient Descent**.  
- New models predict the **Residuals** (negative gradient of the loss function).

---

### 3. Advanced and Hybrid Methods

#### Stacking (Stacked Generalization)
- Uses a **Meta-Model** (Meta-Learner) to learn the optimal way to combine predictions from heterogeneous base models.

#### Voting Classifier/Regressor
- Simplest combination method:  
  - **Hard Voting:** Majority class  
  - **Soft Voting:** Averaging probabilities

---

##  References

1. [DataCamp – Ensemble Learning in Python](https://www.datacamp.com/tutorial/ensemble-learning-python?__cf_chl_rt_tk=dtbvBJ2OjSz.bvOyUG_rlHlStfKr5vGCYSSXH97dpUw-1759690429-1.0.1.1-gLuwOm.dacpCOsTU1Ty49QLFP4TqH3vi9Xid8r9gcFM)  
2. [Medium – Ensemble Methods in Machine Learning](https://ranyel.medium.com/ensemble-methods-in-machine-learning-995a4cb6d825)  
3. [GeeksforGeeks – A Comprehensive Guide to Ensemble Learning](https://www.geeksforgeeks.org/machine-learning/a-comprehensive-guide-to-ensemble-learning/)  
4. [IBM – Ensemble Learning](https://www.ibm.com/think/topics/ensemble-learning)

5. [Decision Trees Explained: Entropy, Information Gain, Gini Index, and CCP Pruning](https://towardsdatascience.com/decision-trees-explained-entropy-information-gain-gini-index-ccp-pruning-4d78070db36c/)  
6. [Introduction to XGBoost in Python](https://blog.quantinsti.com/xgboost-python/)  
7. [Random Forest: Simple Explanation](https://williamkoehrsen.medium.com/random-forest-simple-explanation-377895a60d2d)  
8. [Decision Tree in Machine Learning - GeeksforGeeks](https://www.geeksforgeeks.org/machine-learning/decision-tree/)  
9. [Random Forest Algorithm in Machine Learning - GeeksforGeeks](https://www.geeksforgeeks.org/machine-learning/random-forest-algorithm-in-machine-learning/)  
10. [Scikit-Learn Documentation](https://scikit-learn.org/stable/modules/ensemble.html)
