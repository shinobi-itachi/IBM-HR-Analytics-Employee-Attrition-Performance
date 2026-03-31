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

## Model Selection and Conclusion

To predict employee attrition, multiple machine learning models were trained and evaluated:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Tuned Random Forest (using GridSearchCV)

The models were evaluated using the following classification metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

### Model Comparison

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|------|------|------|------|------|------|
| Logistic Regression | **0.86** | **0.60** | 0.36 | **0.45** | **0.81** |
| KNN | 0.84 | 0.57 | 0.08 | 0.15 | 0.62 |
| Decision Tree | 0.76 | 0.31 | 0.40 | 0.35 | 0.62 |
| Random Forest | 0.84 | 0.50 | 0.08 | 0.14 | 0.79 |
| Tuned Random Forest | 0.83 | 0.47 | 0.29 | 0.36 | 0.76 |

### Key Observations

- **Logistic Regression achieved the best overall performance** across Accuracy, F1 Score, and ROC-AUC.
- **KNN and Random Forest showed very low recall**, meaning they struggled to correctly identify employees likely to leave.
- **Decision Tree showed signs of overfitting**, with weaker generalization performance.
- Random Forest was tuned using **GridSearchCV**, but the tuned model still did not outperform Logistic Regression.

### Final Model Selection

Based on the evaluation results, **Logistic Regression was selected as the final model**.

Reasons for selection:

- Highest overall predictive performance
- Better balance between precision and recall
- Strong ROC-AUC score indicating good classification capability
- Simpler and more interpretable model compared to complex ensemble methods

### Conclusion

The results suggest that the relationship between employee attributes and attrition in this dataset can be effectively captured by a **linear classification model**. Logistic Regression demonstrated the best balance between predictive performance and model simplicity, making it the most suitable model for this problem.

# Business Insights (Markdown)***
• Employees working overtime show significantly higher attrition  
• Lower salary employees tend to leave more often  
• Employees in early career stages show higher turnover  
• Low job satisfaction strongly correlates with attrition
