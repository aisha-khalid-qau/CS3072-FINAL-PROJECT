# CS3072-FINAL-PROJECT
# CS3072 Final Project: Income Prediction Using Demographic and Socioeconomic Data

This repository contains the final project for CS3072, which focuses on using machine learning techniques to predict income categories based on demographic and socioeconomic factors.

## Objective

The objective of this project is to build a predictive model that classifies individuals into two income categories:
- `<=50K`: Annual income less than or equal to $50,000.
- `>50K`: Annual income greater than $50,000.

The analysis aims to identify key factors influencing income levels and provide interpretable insights into these relationships.

---

## Dataset

The project uses the **Adult Dataset** from the UCI Machine Learning Repository. The dataset, derived from the 1994 U.S. Census database, contains features such as:
- **Age**
- **Education Level**
- **Occupation**
- **Hours-per-week**
- **Marital Status**
- **Gender**
- **Native Country**

### Dataset Files
- `data/adult_train.csv`: Training data.
- `data/adult_test.csv`: Testing data.

---

## Methods

### Data Preprocessing
- Handled missing values by imputing the mode for categorical variables.
- One-hot encoded categorical variables and scaled numerical features using StandardScaler.

### Machine Learning Models
1. **Logistic Regression**: Simple and interpretable model.
2. **Random Forest**: A robust ensemble model that handles non-linear relationships.
3. **XGBoost**: A high-performance gradient boosting algorithm.

### Model Evaluation
- Metrics: Accuracy, Precision, Recall, F1-score, and Confusion Matrices.
- Feature Importance: Identified key predictors using Random Forest and XGBoost.
- Interpretability: Used Partial Dependence Plots (PDP) to visualize the relationship between predictors and outcomes.

---

## Results

- **Model Performance**:
  - XGBoost achieved the highest accuracy and F1-score among all models.
  - Random Forest also performed well, while Logistic Regression had lower performance due to linear assumptions.

- **Key Predictors**:
  - Education level, age, and hours worked per week were the most significant features influencing income levels.
  - PDPs highlighted that higher education and more working hours increased the likelihood of earning >$50,000.

---

## Conclusions

The project successfully demonstrated the use of machine learning to predict income categories, with XGBoost emerging as the best-performing model. The analysis provided valuable insights into income disparities and their predictors, aligning with the project's goals.

---

## Limitations and Future Work

### Limitations
- The dataset, being based on 1994 U.S. Census data, may not reflect current socioeconomic trends.
- Class imbalance in income categories could introduce bias despite mitigation efforts.

### Future Work
- Hyperparameter tuning to further optimize model performance.
- Testing on more recent datasets to evaluate the generalizability of the findings.
- Exploring advanced interpretability techniques like SHAP (Shapley Additive Explanations).



