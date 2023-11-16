# credit-risk-classification- Rutgers Data Visualization Bootcamp Module 20
# Summary 
In this challenge, I created two linear regression models for the lending_data.csv provided. These models predicted the "loan_status" value. 
The first model used the original data and received an balanced accuracy  score of .95. However, when we ran RandomOverSampler to make sure the values were equal in our sample, we were able to generate an balanced accuracy score of .99, <br> meaning that this method created a more accurate model. 
# Credit Risk Analysis Report

## Resources
  For this challenge, I referenced the code from the Module 20 class 1 activities. For the RandomOverSampler exercise, I used slack overflow to review the documentation and troubleshoot issues I was having with the RandomOverSampler. to solve this issue, I had to install scikitlearn version 1.21 rather than 1.3.
## Dependencies
python libraries- pandas, numpy, pathlib, sklearn, imblearn.over_sampling - RandomOverSampler, sklearn.metrics
## Author
Allison Potestio
