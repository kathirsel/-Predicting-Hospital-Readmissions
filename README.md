# -Predicting-Hospital-Readmissions
This project aimed to predict hospital readmissions within 30 days. The process involved data preprocessing, feature engineering, model building, and evaluation. The goal was to identify high-risk patients for early intervention, thereby improving patient care. 
# -Predicting-Hospital-Readmissions
 

1. **Data Preprocessing**:  started by making a copy of my DataFrame to avoid modifying the original data.  then normalized several numerical features such as 'Age', 'Num_Lab_Procedures', 'Num_Medications', and 'Total_Visits' using Min-Max normalization. This process scales the range of these features to [0, 1], which can help improve the performance of many machine learning algorithms.

2. **Feature Engineering**: created a new feature 'Total_Visits' by summing up 'Num_Outpatient_Visits', 'Num_Inpatient_Visits', and 'Num_Emergency_Visits'. also engineered a 'High_Risk' feature based on certain conditions like age, diagnosis, number of medications, emergency visits, and readmission status.  then converted categorical variables into numerical using one-hot encoding, which is a common preprocessing step for categorical data.

3. **Model Building**:  split data into training and testing sets using a 70-30 split.then trained a Logistic Regression model on training data. Logistic Regression is a popular choice for binary classification problems like this one.

4. **Model Evaluation**:  evaluated  model on the test data and achieved an accuracy of 51%. 
