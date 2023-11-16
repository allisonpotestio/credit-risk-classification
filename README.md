# credit-risk-classification- Rutgers Data Visualization Bootcamp Module 20
# Summary 
In this challenge, I created two linear regression models for the lending_data.csv provided. These models predicted the "loan_status" value. 
The first model used the original data and received an balanced accuracy  score of .95. However, when we ran RandomOverSampler to make sure the values were equal in our sample, we were able to generate an balanced accuracy score of .99, meaning that this method created a more accurate model. 
# Credit Risk Analysis Report
The purpose of this analysis is to determine which machine learning model should be used to analyze the lending_data.csv provided. <br>
This data included information about 77536, which values including loan size,	interest rate,	borrower income,	debt to income ratio,	number of accounts,	derogatory marks,	total debt,	and loan status loan_status. <br> 
The purpose of this analysis was to predict the loan status based on all the other information about the loan. <br>
If we are able to predict which status the loan will fall into based on these metrics, we may be able to identify parameters of loan approval that need to be changed so that fewer loans are defaulted upon. <br>
We used two methods to create a logistical regression model to predict this data. 


* Method #1 used the original data to create a logistical regression model. This method had a .95 balanced accuracy score. The confusion matrix is listed below. This method was very accurate in predicting the loans in status 0, but not as accurate in predicting the loans in status 1.There was a high proportion of data in status 0 for this model, so in Model #2 we evened out the sample sizes of loans in each status.


<br> precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384
<br>


* Model #2 was able to predict the loan status with a balanced accuracy score of .99. Balancing the sample sizes of each status allowed us to achieve near perfect accuracy. Therefore, I would recommend using this model to predict loan status for future loans.

    precision    recall  f1-score   support

           0       0.99      0.99      0.99     75036
           1       0.99      0.99      0.99     75036

    accuracy                           0.99    150072
   macro avg       0.99      0.99      0.99    150072
weighted avg       0.99      0.99      0.99    150072
## Resources
  For this challenge, I referenced the code from the Module 20 class 1 activities. For the RandomOverSampler exercise, I used slack overflow to review the documentation and troubleshoot issues I was having with the RandomOverSampler. to solve this issue, I had to install scikitlearn version 1.21 rather than 1.3.
## Dependencies
python libraries- pandas, numpy, pathlib, sklearn, imblearn.over_sampling - RandomOverSampler, sklearn.metrics
## Author
Allison Potestio
