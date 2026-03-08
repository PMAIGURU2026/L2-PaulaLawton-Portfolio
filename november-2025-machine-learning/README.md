# November 2025 — Machine Learning Fundamentals

**Month:** November 2025  
**Program:** Pursuit AI Fellowship — Level 2  
**Author:** Paula Lawton

---

## Description

This project dives into supervised machine learning, covering both classification and regression problems. Using `scikit-learn`, the work involved building, evaluating, and improving multiple model types on structured datasets. Special emphasis was placed on understanding the bias-variance tradeoff and proper model evaluation techniques.

## Topics Covered

- Supervised learning: classification vs. regression
- Model types: Logistic Regression, Decision Trees, Random Forests, K-Nearest Neighbors
- Model evaluation: accuracy, precision, recall, F1 score, confusion matrices, ROC-AUC
- Cross-validation and hyperparameter tuning with `GridSearchCV`
- Preprocessing pipelines: `StandardScaler`, `OneHotEncoder`, `Pipeline`

## Project Highlights

- **Customer Churn Prediction:** Built a binary classification model to predict whether a telecom customer would churn. Achieved 83% F1 score on the test set using a tuned Random Forest classifier.
- **Housing Price Regression:** Built a regression model predicting median home values using the Boston/Ames Housing dataset. Compared Linear Regression, Ridge, and Lasso to understand regularization.
- **Pipeline Demo:** Demonstrated how to chain preprocessing and modeling steps into a single `sklearn` Pipeline to prevent data leakage during cross-validation.

## Skills Demonstrated

- Feature selection and importance analysis
- Avoiding data leakage through proper train/test splitting and pipelines
- Documenting model performance with comparison tables

## How to Run

```bash
pip install scikit-learn pandas numpy matplotlib seaborn jupyter

jupyter notebook
```

## Key Takeaways

Model selection is only a small part of the work — feature engineering, evaluation strategy, and preventing data leakage matter far more. A well-constructed baseline model is always the right starting point before reaching for complex ensembles.
