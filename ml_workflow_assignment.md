Task 1: Label and Data Leakage

Label column: repeat_purchase_flag
Justification: This is the target variable — it directly encodes the outcome we're trying to predict (whether a customer made a repeat purchase within 30 days).

Data leakage column: discount_used_on_repeat_order
Justification: This column contains information about the repeat purchase order itself, meaning it's only known after the target event has occurred — including it as a feature would leak future information into the model.

Task 2: Two ML Workflow Steps Before Gradient Boosting

1. Exploratory Data Analysis (EDA)
Before training any model, it is important to explore the dataset to understand distributions, detect missing values, identify outliers, and check relationships between variables. This helps in making better feature selection and avoiding incorrect assumptions.

2. Data Preprocessing and Feature Engineering
Data should be cleaned and prepared by handling missing values, encoding categorical variables, and scaling if required. Proper preprocessing ensures that the model learns meaningful patterns and improves overall performance.