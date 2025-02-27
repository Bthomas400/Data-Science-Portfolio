Interconnect Churn Model

Overview

Interconnect, a telecom provider, faces a customer churn issue, where users progressively leave the service. Since retaining customers is more cost-effective than acquiring new ones, this project aims to develop a predictive model to identify customers at risk of churn. The model evaluates historical contract data, demographics, and service usage to predict churn likelihood. The primary evaluation metric is the AUC-ROC score, with a target of at least 0.75 to ensure robust classification.

Technologies Used

Python: Main programming language for the project.

Pandas & NumPy: Data manipulation and preprocessing.

Matplotlib & Seaborn: Data visualization.

Scikit-Learn: Implementation of machine learning models, preprocessing, and evaluation.

Jupyter Notebook: Interactive computing environment.

Key Findings

Model Performance: The final Gradient Boosting model achieved an AUC-ROC score of 0.8625, exceeding the initial target.

Feature Importance: Key factors influencing churn include contract type, payment method, and tenure duration.

Predictive Accuracy: The model effectively distinguishes between churn and non-churn customers, validated by both AUC-ROC and accuracy metrics.

Data Preparation

The dataset includes four key sources:

Contract Data: Details on contract type, payment method, monthly charges, and tenure.

Personal Data: Customer demographics such as gender, age, and partner status.

Internet Data: Internet service details, including security, backup, and streaming options.

Phone Data: Multiple line subscriptions and phone service usage.

Data Processing Steps:

Handling Missing Values: Imputed missing entries with appropriate replacements (e.g., "No Service").

Feature Engineering: Created tenure-based insights and converted categorical features into numerical representations.

One-Hot Encoding: Encoded categorical variables for better model interpretability.

Scaling: Standardized numerical features such as monthly charges and total charges.

Model Development

Models Evaluated:

Logistic Regression (Baseline Model)

Random Forest Classifier (Hyperparameter-tuned with GridSearchCV)

Gradient Boosting Classifier (Final selected model)

Techniques Implemented:

Hyperparameter Tuning: GridSearchCV optimized Random Forest and Gradient Boosting parameters.

Data Imbalance Handling: Addressed imbalance by adjusting class weights and feature selection.

Performance Comparison:

Model

AUC-ROC Score

Accuracy

Logistic Regression

0.8546

81.83%

Random Forest

0.8625

80.26%

Gradient Boosting

0.8624

81.41%

Conclusion

The Gradient Boosting model was selected as the final model due to its strong predictive performance and ability to identify at-risk customers effectively.

Business Impact:

Targeted Customer Retention Strategies: Focus on customers with month-to-month contracts and high-risk payment methods.

Service Improvement: Address churn drivers by enhancing support and providing additional customer incentives.

Predictive Insights: Deploy the model in Interconnect’s CRM system for proactive retention efforts.

Next Steps:

Integrate the model into a real-time churn monitoring system.

Further optimize hyperparameters for even better prediction accuracy.

Explore deep learning techniques for future model improvements.
