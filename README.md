### Data Analysis on Customer Attrition Prediction

#### 1. Introduction
The aim of this analysis is to predict customer attrition (churn) based on various attributes of customers, such as demographic information, transaction history, and account information. The data includes customer demographics, credit card usage, and other behavioral indicators.

#### 2. Dataset Description
The dataset contains various attributes:
- **CLIENTNUM**: Client number
- **Attrition_Flag**: Whether the customer is attrited (churned) or existing
- **Customer_Age**: Age of the customer
- **Gender**: Gender of the customer
- **Dependent_count**: Number of dependents
- **Education_Level**: Education level of the customer
- **Marital_Status**: Marital status of the customer
- **Income_Category**: Income category of the customer
- **Card_Category**: Type of credit card
- **Months_on_book**: Duration in months the customer has been on the books
- **Total_Relationship_Count**: Total number of products held by the customer
- **Months_Inactive_12_mon**: Number of months inactive in the last 12 months
- **Contacts_Count_12_mon**: Number of contacts in the last 12 months
- **Credit_Limit**: Credit limit of the customer
- **Total_Revolving_Bal**: Total revolving balance on the credit card
- **Avg_Open_To_Buy**: Average open to buy credit line
- **Total_Amt_Chng_Q4_Q1**: Change in transaction amount (Q4 over Q1)
- **Total_Trans_Amt**: Total transaction amount
- **Total_Trans_Ct**: Total transaction count
- **Total_Ct_Chng_Q4_Q1**: Change in transaction count (Q4 over Q1)
- **Avg_Utilization_Ratio**: Average utilization ratio

#### 3. Data Preprocessing
To ensure the data is suitable for machine learning models, preprocessing steps were applied:
- **Handling Missing Values**: Missing values were imputed using the mean value of the respective columns.
- **Encoding Categorical Variables**: Categorical variables such as Gender, Education_Level, Marital_Status, Income_Category, and Card_Category were converted to dummy variables using one-hot encoding.
- **Feature Scaling**: Numeric features were scaled to ensure they are on a similar scale (not shown but implied in good practice).

#### 4. Model Training and Evaluation
A RandomForestClassifier was used to predict customer attrition. The steps included:
- **Data Splitting**: The dataset was split into training (80%) and testing (20%) sets.
- **Model Training**: The RandomForestClassifier was trained on the training data.
- **Model Evaluation**: The model was evaluated using the test data. Metrics included confusion matrix, classification report, and accuracy score.

#### 5. Feature Importance
Feature importance was assessed to understand the impact of each feature on the prediction. The most important features included:
- Total_Trans_Ct
- Total_Trans_Amt
- Total_Relationship_Count
- Total_Amt_Chng_Q4_Q1

These features were critical in predicting whether a customer would churn or remain with the company.

#### 6. Predictions for New Data
A sample prediction was made for new customer data. This involved imputing missing values in the new data and then using the trained model to predict whether the customer would churn.

#### 7. Visualization
Several visualizations were created to better understand the data:
- **Heatmaps**: To show the relationship between frequency and monetary values with churn rate and number of users.
- **KDE and Box Plots**: To visualize the distribution of key features by attrition flag.

#### 8. Conclusion
The analysis provided valuable insights into the factors that influence customer attrition. By identifying key attributes and understanding their impact, the company can develop strategies to improve customer retention. The RandomForestClassifier proved effective in predicting customer churn, and the visualization tools helped to clarify the data trends and relationships.

#### Key Takeaways
- **High transaction counts and amounts** are strong indicators of customer retention.
- **Frequent contact and engagement** with the company correlate with lower attrition.
- **Education and income levels** also play a role in customer behavior, affecting churn rates differently across various segments.

Overall, this analysis highlights the importance of understanding customer behavior through comprehensive data analysis and predictive modeling.
