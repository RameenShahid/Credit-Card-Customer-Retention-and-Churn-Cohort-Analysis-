# 📊 Data Analysis on Customer Attrition Prediction

## 🔍 1. Introduction
Customer attrition, or churn, is a key concern for financial institutions. This analysis aims to predict customer churn based on demographic details, transaction history, and account usage. The dataset includes customer demographics, credit card behavior, and engagement patterns.

---

## 📁 2. Dataset Description
The dataset contains the following attributes:

🆔 **CLIENTNUM**: Unique client identifier  
🔄 **Attrition_Flag**: Status (churned or existing customer)  
🎂 **Customer_Age**: Customer's age  
🚻 **Gender**: Customer's gender  
👨‍👩‍👧 **Dependent_count**: Number of dependents  
🎓 **Education_Level**: Customer's education level  
💍 **Marital_Status**: Marital status  
💰 **Income_Category**: Customer's income range  
💳 **Card_Category**: Type of credit card held  
📅 **Months_on_book**: Duration (in months) the customer has held the account  
🔗 **Total_Relationship_Count**: Number of products held by the customer  
🕒 **Months_Inactive_12_mon**: Months inactive in the past year  
📞 **Contacts_Count_12_mon**: Customer service contacts in the past year  
🏦 **Credit_Limit**: Customer’s credit limit  
💳 **Total_Revolving_Bal**: Total revolving balance  
📈 **Avg_Open_To_Buy**: Available credit line  
📊 **Total_Amt_Chng_Q4_Q1**: Change in transaction amount (Q4 vs. Q1)  
💵 **Total_Trans_Amt**: Total transaction amount  
🔢 **Total_Trans_Ct**: Total transaction count  
📉 **Total_Ct_Chng_Q4_Q1**: Change in transaction count (Q4 vs. Q1)  
⚖ **Avg_Utilization_Ratio**: Average credit utilization ratio  

---

## 🛠 3. Data Preprocessing
To ensure high-quality data, the following preprocessing steps were applied:

✅ **Handling Missing Values**: Imputed using column mean values  
✅ **Encoding Categorical Variables**: Converted to dummy variables using one-hot encoding  
✅ **Feature Scaling**: Normalized numeric features for uniformity  

---

## 🤖 4. Model Training and Evaluation
A **RandomForestClassifier** was used for prediction, following these steps:

📌 **Data Splitting**: 80% training, 20% testing  
📌 **Model Training**: RandomForestClassifier trained on the dataset  
📌 **Model Evaluation**: Measured using confusion matrix, classification report, and accuracy score  

---

## 🔥 5. Feature Importance
Feature importance analysis highlighted the most influential variables:

🔹 **Total_Trans_Ct**  
🔹 **Total_Trans_Amt**  
🔹 **Total_Relationship_Count**  
🔹 **Total_Amt_Chng_Q4_Q1**  

These features played a significant role in predicting churn probability.

---

## 🔮 6. Predictions for New Data
For new customer data, missing values were handled, and the trained model was used to predict churn likelihood.

---

## 📊 7. Visualization
To better understand churn trends, various visualizations were generated:

🔥 **Heatmaps**: Showed correlations between features and churn rate  
📊 **KDE & Box Plots**: Displayed feature distributions across churn status  

---

## 🏆 8. Conclusion
This analysis provided deep insights into customer attrition. By identifying influential factors, businesses can implement strategies to enhance customer retention. The **RandomForestClassifier** proved effective in predicting churn, while visualizations helped uncover patterns in customer behavior.

### 🎯 Key Takeaways
✔ **Higher transaction counts and amounts** indicate lower churn probability  
✔ **Frequent customer engagement** reduces attrition risk  
✔ **Education & income levels** influence churn differently across customer segments  

📢 **Actionable Strategy:** Enhance customer engagement and offer targeted incentives to reduce churn. 

🚀 **Future Work:** Explore advanced models like XGBoost and deep learning to improve prediction accuracy.



#### Key Takeaways
- **High transaction counts and amounts** are strong indicators of customer retention.
- **Frequent contact and engagement** with the company correlate with lower attrition.
- **Education and income levels** also play a role in customer behavior, affecting churn rates differently across various segments.

Overall, this analysis highlights the importance of understanding customer behavior through comprehensive data analysis and predictive modeling.
