# predictRisk

Machine Learning python model to predict low, medium or high risk for financial loans

## Background

The model uses the ```sklearn``` package to train and then ```LogisticRegression``` and ```predict``` to provide the prediction of level of risk.

## Training for model
The model was trained using a script that created 500,000 rows with the following values:

The following variables were used:
*  mortgage_payment: Random integers between 850 and 5500.
*  credit_score: Random integers between 500 and 850.
*  dti_ratio: Random floats between 0.00 and 0.65, rounded to 2 decimal places.
*  annual_salary: Random integers between 57000 and 2105000.
*  risk_level: Determined based on the specified conditions. If the conditions for a low risk are not met, the risk is randomly chosen as 'low', 'medium', or 'high'.

Some background on the constraints:
*  If credit_score is greater than 735 and dti_ratio is less than 0.33 and annual_salary is above 65000 and mortgage_payment is less than 1200, risk is low.
*  If credit_score is greater than 735 and dti_ratio is less than 0.33 and annual_salary is above 255000 and mortgage_payment is less than 2500, risk is low.
*  If credit_score is greater than 720 and dti_ratio is less than 0.33 and annual_salary is above 535000 and mortgage_payment is less than 4200, risk is low.
*  The rest has been calculated randomly.
