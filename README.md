# Smart Loan Recovery System with Machine Learning

This project uses Machine Learning to identify borrowers who are likely to default on their loans. Based on the borrower's profile and repayment behavior, the system recommends the best recovery strategy.

## Project Summary

The system helps financial institutions:
- Understand borrower risk levels
- Group borrowers into segments
- Predict high-risk borrowers
- Recommend a recovery method based on risk

## What the Dataset Contains

The dataset includes the following details:
- Borrower details like age, income, and employment type
- Loan details like amount, tenure, interest rate, and collateral value
- Repayment history like missed payments, EMI, and days past due
- Recovery status (fully recovered, partially, or not recovered)
- Collection attempts and whether legal action was taken

## Steps Followed in the Project

1. Import the dataset using pandas  
2. Visualize loan amount vs income, payment history, and missed payments  
3. Cluster borrowers using K-Means into 4 segments based on financial behavior  
4. Label high-risk segments (for example, high loan + low income = high risk)  
5. Train a Random Forest model to predict high-risk borrowers  
6. Predict risk score and classify new borrowers as high or low risk  
7. Recommend recovery strategy:
   - High risk: legal notices and aggressive recovery  
   - Moderate risk: settlement offers and repayment plans  
   - Low risk: reminders and monitoring  
