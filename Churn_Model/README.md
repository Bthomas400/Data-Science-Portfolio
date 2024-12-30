# Beta Bank Customer Retention Model

## Overview
Beta Bank is experiencing a customer churn issue, with customers progressively leaving the bank. As retaining existing customers is more cost-effective than acquiring new ones, this project aims to develop a predictive model to identify customers at risk of churn. Using historical behavior and contract termination data, the model evaluates the likelihood of customers leaving the bank. The primary evaluation metric is the F1 score, with a target of at least 0.59, complemented by the AUC-ROC metric to ensure comprehensive performance assessment.

## Technologies Used
- **Python**: Main programming language for the project.
- **Pandas**: Data manipulation and analysis.
- **Matplotlib**: Data visualization.
- **Scikit-Learn**: Implementation of machine learning models, data preprocessing, model evaluation, and pipeline creation.
- **Jupyter Notebook**: Interactive computing environment.

## Key Findings
- **Model Performance**: The final Random Forest model achieved an F1 score above the target, indicating a strong predictive performance.
- **Feature Importance**: Key features influencing customer churn include age, balance, number of products, and credit score.
- **Predictive Accuracy**: The model's AUC-ROC score validates its effectiveness in distinguishing between the customer classes.

## Data Preparation
Data involves processing steps including handling missing values, encoding categorical variables, and scaling numerical features to prepare for model training. Detailed data insights revealed the need for balancing the classes, leading to techniques such as upsampling being implemented.

## Model Development
Several models were evaluated, including Logistic Regression, Decision Tree, and Random Forest, with the latter providing the best performance after hyperparameter tuning and class balancing. Techniques to address class imbalance included:
- **Class weight adjustment**: To penalize mistakes on the minority class more heavily.
- **Upsampling the minority class**: To artificially balance the class distribution.

## Conclusion
The Random Forest model, with adjusted class weights and upsampling, provided the highest F1 score, making it suitable for deployment. Beta Bank can utilize this model to identify at-risk customers and potentially offer targeted interventions to improve retention rates.

