Predicting Bank Customer Attrition through Transactional Data
Author:  Matt Linderman

Executive Summary:  The cost of losing and having to acquire customers in banking is large and challenging.  There can be many reasons for the attrition of customers and if we can proactively understand those, we can potentially take action to mitigate that risk through engagement with those customers in question.  The goal of this exercise is to create a model that will allow us to predict those customers likely to attrite – and to do so with transactional data that would be readily available as part of our ongoing business operations.

Rationale:  having a model that is interpretable and allows for predicting the likelihood of attrition will allow us to take actions to retain customers which will be substantially less expensive than the cost and impact of losing and/or having to reacquire customers.

Research Question:   is it possible, using readily available transactional data, to predict the customers that are likely to attrite.

Data Sources:  the primary data source for this exercise has been extracted from our core banking platform and includes a number of features and some level of historical (past 6 months) values to allow for looking at both magnitude and change as variables.

Data & Preparation:  For this exercise, we are using live data (non-sensitive with no identifiable features) for a sample of approximately 40,000 customers – both that have closed accounts and those that remain open as of this extract.

Methodology:  For this exercise, we will first analyze and cleanse/prepare the data and we will then build an initial simplistic machine learning model.   We will initially be using a logistic regression model due to it’s simplicity and interpretability which will be important.

Results:  As a result of this exercise, we are encouraged that we can develop a valuable model to predict customer attrition.  While our initial results are not yet great, we believe we can continue to refine this model and improve our results.  Additionally, unlike some use cases, the predictions of customers that may attrite that are inaccurate, the actions that might be taken to mitigate attrition (albeit not necessary) are likely low cost and no-regret moves.

Next Steps:   Post the completion of this initial exercise, we will be focused on additional feature engineering and optimizing which features the model is using. 
To provide a few examples, we will look at using tools and tactics to select the most relevant features using things like LASSO regularization.  Additionally, we will look to optimize hyperparamerts looking at things like GridSearch and RandomSearch to improve model performance.  Finally, we will consider data scaling as well given the wide range of numerical values within our dataset.

Outline of the Project:
Jupyter Notebook (in this directory)
Data Set Used (cust_data.csv in this directory)

That dataset can be found in the GitHub directory:
cust_data.csv
The target variable within this dataset is “closed_ind” in which a “1” denotes a closure and a “0” denotes open.
The details of data preparation can be found within the Jupyter notebook found in this directory.
