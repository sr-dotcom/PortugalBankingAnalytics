# PortugalBankingAnalytics
This repository houses the machine learning models and analyses used in predicting the likelihood of bank clients subscribing to term deposits. By analyzing factors such as client demographics, past campaign data, and client-bank interactions, we aim to optimize future marketing strategies and improve client targeting.

**Problem Statement** 
The data is related to direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. 

In this project, you need to build a model for deciding whether a campaign will be successful in getting a client to sign up for the term deposits.

**Dataset Description:**

Bank client data

1.**age** (numeric)

2.**job**:typeofjob(categorical:'admin.','bluecollar','entrepreneur','housemaid','management','retired','selfemployed','services','student','technician','unemployed','unknown')

3.**marital**: marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)

4.**education**: (categorical "unknown","secondary","primary","tertiary")

5.**default**: has credit in default? (binary: "yes","no")

6.**balance**: average yearly balance, in euros (numeric) 

7.**housing**: has housing loan? (binary: "yes","no")

8.**loan**: has personal loan? (binary: "yes","no")
 

Data related to the last contact of the current campaign

1.**contact**: contact communication type (categorical: "unknown","telephone","cellular")

2.**day**: last contact day of the month (numeric)

3.**month**: last contact month of year (categorical: "jan", "feb", "mar", ..., "nov", "dec")

4.**duration**: last contact duration, in seconds (numeric)
 

Other attributes:

1.**campaign**: number of contacts performed during this campaign and for this client (numeric, includes last contact)

2.**pdays**: number of days that passed by after the client was last contacted from a previous campaign (numeric, -1 means client            was not previously contacted)

3.**previous**: number of contacts performed before this campaign and for this client (numeric)

4.**poutcome**: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')
 

Output variable (desired target):

**y**: has the client subscribed a term deposit? (binary: "yes","no")
 

**Objectives:**

You are required to prepare a well-commented an interactive python notebook as your solution to this problem statement. The notebook must meet the following objectives:

1.Clean the data and drop useless columns.

2.Make an EDA report, i.e., perform a univariate and bivariate analysis. Also, derive new features based on the given features,   remove outliers and correlated variables if necessary.

3.Visualize the distributions of various features and correlations between them.

4.Perform feature engineering to extract the correct features for the model.

5.Build a logistic regression model

6.Evaluate the model used.

 
**Model Evaluation:**

When you're done with the model building and residual analysis and have made predictions on the test set, just make sure you use **y_test and y_pred.**

where **y_test** is the test data set for the target variable, and **y_pred** is the variable containing the predicted values of the target variable on the test set. Also, remember if the VIF for the selected features is not coming high always check the p-values of the variables before applying the model on test data.

**Dataset:**

* File Name "bank" contains information related to direct marketing campaigns of a banking institution, where the primary mode     of contact is phone calls. The goal seems to be predicting whether a client will subscribe to a term deposit, as indicated by   the 'y' column. 
