# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of the machine learning analysis is to develop a model that can confidentally predict the risk associated with health loans (0) and high risk loans (1). The machine learned from previous lending features such as the size of a loan, the income of the borrower, how high the borrowers interest rate was set to be, the debt to income ratio for each borrower, and the number of accounts the borrower has. These variables were used to predict the likelyhood of the borrower not being able to payback their loan or in other works the risk that the bank would be taking lending to borrowers. 

To develop the machine learning process I started by importing all of my dependenies and reading all of the data from the csv file. Once this was done I seperated the models lables (loan_status) and the features the model would be utilizing (all other columns of data). Then via train_test_split, I had the machine split the data into x and y train/test dat which the model uses to learn and make its predictions. I then moved on to having the machine adjust the train and test data to fit into the parameters of the model in order to create its predictions, with minimal differences between the the actual data provided and the predictions. The model was fit via SKLearns Logistic Regression which creates preidictions for a binary outcome, in our case 0 indicates healthy loans while 1 represents higher risk loans. 


## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
        * Accuracy: 0.99 -> this is a high score indicating that the prediciton model is highly accurate 
        * Precision: (0) 0.99 -> this is a high precision score indicating that the model has a high count of true positives 
        * Recall: (0) 1.00 -> This is an excellent recall score and indicates the models ability to correctly identify true positives for healthy loans. In addition this contributes to the models high precision score.
        * Precision: (1) 0.94 -> this is a high precision score indicating that the model has a high count of true positives. However, this is lower than the precision score for healthy loans, indicating that the model is less precise when predicting the risk rate for high risk loans to borrowers. 
        * Recall: (0) .90 -> This is still an excellent recall score and however is lower than the recall score for healthy loans, which contributes to less precession when predicting risk for high risk loans.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
Based on the classification reports precision rates the model works best when predicting the risk rate for healthy loans. In this case it would be more important for the stakeholder to have the model more confidentally predict the risk for higher risk loans since there is more at stake. Since the model can still predict for the high risk with high precision, I would still recommend utilizing the model for both healthy and high risk loans. 
