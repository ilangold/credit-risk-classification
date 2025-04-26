# Credit Risk Classification
Module 20 Challenge - Supervised Learning

### Analysis Overview
The purpose of this analysis is to predict the health of loans in a peer-to-peer lending service. The analysis uses financial data such as the loan size and interest, as well as borrower income, debt, and derogatory marks to classify each loan as healthy (unlikely to default) or high-risk (likely to default). The end result is a model that predicts the loan status which can then be compared to the known loan status, also included in the data.

The analysis first loads the loan data into a dataframe and separates the known loan status column from the rest of the data. The whole dataset is then separated into training and testing data using scikitlearn. A logistic regression linear model is prepared and fit to the training data, creating a classifier model. This classifier is then used to make predictions on the test data which are compared to the actual loan status from the test data.

### Results
- Healthy Loans
    - Accuracy: 100%
    - Recall: 100%
    - f1-score: 100%
- High-risk Loans
    - Accuracy: 87%
    - Recall: 95%
    - f1-score: 91%
- Overall Accuracy: 99%

### Summary
This model is very usefull, with an overall accuracy of 99%. I would recommend the peer-to-peer lending service use this model to track the active loans on their platform for potentially high-risk loans. The model would very quickly provide the company with a way to identify loans that may default and give them an opportunity to contact the involved parties for a more detailed assessment of the loan. Because of the moderate accuracy in predicting high-risk loans (13% of predicted high-risk loans were not defaulted on), this model should only be used for exploratory analysis. It would be an appropriate model for directing investigation and sending inquiries, not warnings or collections threats.
