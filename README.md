Case Study Dataset
The data set Churn is based on the customers of a single bank in Europe. It 
contains 10,000 observations and 17 variables. Each observation indicates a 
customer and the 17 variables describe their characteristics. Detail of each variable 
is described in Table 1. You have been hired as a data analyst consultant by the 
bank. Your task is to inform decision-makers of the (characteristics of) customers 
using their attributes to predict which customers are likely to exit and stop using the 
banking services.
Table 1: List of Variables
Attribute Description
RowNumber Observation identification number
CustomerID Customer’s identification number
Surname Surname of the customer
CreditScore The latest credit score of the customer
Geography Customer’s country where the bank account is opened
Gender Customer’s gender
Sex Customer’s sex (0-male or 1-female)
Age Customer’s age
CurrentWorkingStatus Customer’s current status of working (1-working or 0-
not working)
Tenure Customer’s duration of active relationship with the bank
Balance Balance money currently available in the customer’s 
bank account
NumOfProducts Total number of products that the customer benefits 
from the bank
ComplaintsLodged Represents if the customer has lodged a complaint 
previously (1-yes or 0-no)
HasCrCard Represents if the customer has a credit card or not (1-
yes or 0-no) 
IsActiveMember Represents if the customer is an active member (1-yes 
or 0-no)
EstimatedSalary An estimated salary of the customer
Exited Represents if the customer stayed or exited and 
stopped using the banking services (Yes-exited or Nostayed)
Case Study Tasks
Your task is to build various predictive models including decision tree, regression 
function, and neural network on this data set and compare them. Results inferred by 
these models should inform decision-makers of the (characteristics of) customers
who have a high risk of churn. This information can be utilized in multiple ways to 
assist various stakeholders. 
Specific tasks for each data analytics process are listed below.
Task 1. Data Selection and Distribution. (4 marks)
1. What is the proportion of customers who exited and stopped using the 
banking services?
2. The dataset may include irrelevant and redundant variables. What 
variables did you include in the analysis and what were their roles and 
measurement level set? Justify your choice.
3. Did you have to fix any data quality problems? Detail them.
Apply the imputation method(s) to the variable(s) that need it. List the
variables that needed it. Justify your choice of imputation if needed.
4. Report the proportion of values of the target variable for the dataset after 
the above-mentioned pre-processing. 
5. What distribution split between training and test datasets have you 
used?
Task 2. Predictive Modeling Using Decision Trees (4 marks)
1. Build a decision tree using the default setting. Examine the tree results and
answer the following:
a. What parameters have been used in building the tree? Detail them.
b. What is classification accuracy on training and test datasets?
c. What is the size of the tree (number of nodes and rules)?
d. Which variable is used for the first split? What are the variables that 
are used for the second split?
e. What are the 5 important variables in building the tree? 
f. Report if you see any evidence of model overfitting. 
2. Build another decision tree tuned with GridSearchCV. Examine the tree
results.
a. What are the optimal parameters for this decision tree?
b. What is classification accuracy on training and test datasets?
c. What is the size of the chosen tree (number of nodes and rules)?
d. Which variable is used for the first split? What are the variables that 
are used for the second split?
e. What are the 5 important variables in building the tree? 
f. Report if you see any evidence of model overfitting. 
3. What is the significant difference do you see between these two decision tree 
models – default (Task 2.1) and using GridSearchCV (Task 2.2)? How do they 
compare performance-wise? Explain why those changes may have happened.
4. From the better model, can you provide a descriptive summary of customers 
that most likely exit and stop using the banking services? 
Task 3. Predictive Modeling Using Regression (5.5 marks)
1. Describe what and why you will have to do additional preparation for variables 
to be used in regression modelling. List the variables that needed it with the 
processing detail.
2. Build a regression model using the default regression method with all 
inputs. Once you have completed it, build another model and tune it using 
GridSearchCV. Answer the following:
a. Name the Regression function used.
b. Report the variables that are included in the regression model.
c. Report the top-5 important variables (in order) in the model.
d. What is classification accuracy on training and test datasets? Report 
any sign of overfitting.
3. Build another regression model using the subset of inputs selected by RFE. 
Answer the following:
a. Was dimensionality reduction useful to identify a good feature set for 
building the accurate model?
b. Report the variables that are included in the regression model.
c. What is classification accuracy on training and test datasets? Report 
any sign of overfitting.
4. Using the comparison statistics, which of the regression models appears to 
be better? Explain why.
5. From the better model, can you provide a descriptive summary of customers 
that most likely exit and stop using the banking services?
Task 4. Predictive Modeling Using Neural Networks (5.5 marks)
1. Build a Neural Network model using the default setting. Answer the 
following:
a. What are the parameters used, e.g., network architecture, iterations, 
activation function, etc? 
b. What is the classification accuracy on training and test datasets?
c. Comment on the training process concerning underfitting, overfitting 
or good fitting.
2. Refine this network by tuning it with GridSearchCV. Answer the 
following:
a. What are the parameters used, e.g., network architecture, iterations, 
activation function, etc? 
b. What is the classification accuracy on training and test datasets?
c. Comment on the training process concerning underfitting, overfitting 
or good fitting.
3. Would feature selection help here? Build another Neural Network model 
with inputs selected from RFE with regression (use the best model
generated in Task 3) and from the decision tree (use the best model 
from Task 2). Tune the model with GridSearchCV to find the best 
parameters setting. Answer the following for the best neural network 
model:
a. Did feature selection help here? Which method of feature selection 
produced the best result? Any change in the network architecture? 
What inputs are being used as the network input?
b. What is classification accuracy on training and test datasets? Is there
any improvement in the outcome?
c. How many iterations are now needed to train this network?
d. Comment on the training process concerning underfitting, overfitting 
or good fitting.
4. Using the comparison statistics, which of the Neural Network models 
appears to be better? 
5. From the better model, can you provide a descriptive summary of 
customers that most likely exit and stop using the banking services?
Task 5. Comparing Predictive Models (4 marks)
1. Use the comparison statistics to compare the best decision tree model, the 
best regression model, and the best neural network model. 
a. Discuss the findings led by:
(i) ROC Chart and Index; 
(ii) Accuracy Table; 
b. Which model would you use in deployment based on these findings? 
Discuss why?
2. Can you summarise the positives and negative aspects of each predictive 
modelling method based on this data analysis exercise? 
3. Finally, can you build an ensemble model combining all models? Does it 
produce better/equal/worse performance and why?
