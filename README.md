# Email-Campaign-Effectivness

In this project, I have attempted to analyze the data on e-mail marketing campaign and build a machine learning model to predict the mail that is ignored, read, or acknowledged by the reader. No personal information of recipient is provided in this dataset.

#  Problem Statement

Most of the small to medium business owners are making effective use of Gmail-based e-mail marketing strategies for offline targeting of converting their prospective customers into leads so that they stay with them in business. The main objective is to create a machine learning model to characterize the mail and track the mail that is ignored; read; acknowledged by the reader.

# Approach

Understanding the business task.
Import relevant libraries and define useful functions.
Reading data from files given.
Data pre-processing, which involves inspection of both datasets and data cleaning.
Exploratory data analysis, to find which factors affect sales and how they affect it.
Feature engineering, to prepare data for modelling.
Modelling data and comparing the models to find out most suitable one for classification.
Conclusion.

# Exploratory Data Analysis
The following insights were gained from EDA:

Less number of e-mails of campaign type 1 got ignored.
If campaign type is 1, then the mail has 66% chance of getting read and 23% change of getting acknowledged.
Customer location or time of day does not affect the status of e-mail.
As the number of previous communication increases, the chances of the e-mail being read or acknowledged also increases.
E-mails tend to get ignored when word count is greater than 800.

# Conclusion
The following conclusions were drawn from Modelling:

Oversampled data seems to be better than undersampled data. This can be due to the fact that undersampling causes loss of information.
The model built using XGBoost algorithm with SMOTE dataset performed better than the other models. It should be preferred for predicting mail statuses.
If model interpretability is more important than accuracy, model built using logistic regression algorithm and SMOTE dataset should be chosen over the one using XGBoost algorithm. It is the best performer among the white box models.
