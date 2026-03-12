# IBM-HR-Analytics-Employee-Attrition-Performance
End-to-end machine learning project to predict employee attrition using Logistic Regression, KNN, Decision Tree, and Random Forest with hyperparameter tuning, ROC-AUC evaluation, and employee segmentation using K-Means clustering.


# Employee Attrition Prediction & Employee Segmentation

Machine Learning project to predict employee attrition and segment employees using clustering.

Author: Rohit Kamble  
Target Role: Machine Learning Engineer

---

# Problem Statement

Employee attrition leads to increased hiring costs and productivity loss.  
The objective of this project is to predict employee attrition using machine learning models and provide insights into workforce patterns.

---

# Dataset

IBM HR Analytics Employee Attrition Dataset

Rows: 1470  
Features: 35  

Target variable: Attrition

---

# Project Pipeline

1. Data Collection
2. Exploratory Data Analysis
3. Feature Engineering
4. Feature Selection
5. Model Training
6. Model Evaluation
7. Hyperparameter Tuning
8. ROC-AUC Analysis
9. K-Means Employee Segmentation
10. Final Model Selection

---

# Exploratory Data Analysis

## Attrition Distribution

![Attrition Distribution](images/attrition_distribution.png)

---

# Model Performance

| Model | Accuracy | Recall | ROC-AUC |
|------|------|------|------|
| Logistic Regression | 0.82 | 0.64 | 0.84 |
| KNN | 0.80 | 0.60 | 0.82 |
| Decision Tree | 0.83 | 0.67 | 0.85 |
| Random Forest | **0.86** | **0.72** | **0.89** |

Final model: Random Forest (tuned)

---

# ROC Curve

![ROC Curve](images/roc_curve.png)

---

# Feature Importance

![Feature Importance](images/feature_importance.png)

Key drivers of attrition:

- Overtime
- Monthly Income
- Job Satisfaction
- Years At Company

---

# Employee Segmentation

Using K-Means clustering we segmented employees into workforce groups.

![Clusters](images/clusters.png)

Insights:

- Young employees show higher attrition
- Employees with overtime have higher exit risk
- Experienced employees show lower attrition

---

# Technologies Used

Python  
Pandas  
Scikit-learn  
Seaborn  
Matplotlib  

---

# Future Improvements

- Build API using Flask
- Deploy model
- Create HR dashboard
