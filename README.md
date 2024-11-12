# Credit Risk Classification 
The credit risk classification looks to utilize machine learning to categorize the risk of loaning to borrwers based on feautures including the size of a loan, the income of the borrower, how high the borrowers interest rate was set to be, the debt to income ratio for each borrower, and the number of accounts the borrower has. 

# Dependencies 
1. Numpy 
2. Pandas
3. Pathlib
4. sklearn.metrics

# Results
The models results were prediction utilizing SKLearns Logistic Regression which creates preidictions for a binary outcome, in our case 0 indicates healthy loans while 1 represents higher risk loans. 
- Accuracy: 0.99 -> this is a high score indicating that the prediciton model is highly accurate 
- Precision: (0) 0.99 -> this is a high precision score indicating that the model has a high count of true positives 
- Recall: (0) 1.00 -> This is an excellent recall score and indicates the models ability to correctly identify true positives for healthy loans. In addition this contributes to the models high precision score.
- Precision: (1) 0.94 -> this is a high precision score indicating that the model has a high count of true positives. However, this is lower than the precision score for healthy loans, indicating that the model is less precise when predicting the risk rate for high risk loans to borrowers. 
- Recall: (0) .90 -> This is still an excellent recall score and however is lower than the recall score for healthy loans, which contributes to less precession when predicting risk for high risk loans.

# Summary 
Based on the classification reports precision rates the model works best when predicting the risk rate for healthy loans. In this case it would be more important for the stakeholder to have the model more confidentally predict the risk for higher risk loans since there is more at stake. Since the model can still predict for the high risk with high precision, I would still recommend utilizing the model for both healthy and high risk loans. 


# Resources 
- * `lending_data.csv`
