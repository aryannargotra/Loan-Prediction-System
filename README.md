# Loan-Prediction-System
Data Science Assignment - REUNION


File named Data Insights

Task 1

1. Do the Exploratory Data Analysis & share the insights.

Firstly read both csv files and did the exploratory analysis of both checked the relationship 
between the Number of existing loans at this bank with High Risk applicant and bivariate analysis of Principal_loan_amount and Balance_in_existing_bank_account_(lower_limit_of_bucket)


2. How would you segment customers based on their risk (of default)?

Merged the Applicant and Loan dataframes then removed the non essential columns merged Applicant Id and High risk applicant column in same table ordered by their risk.

3. Which of these segments / sub-segments would you propose be approved?

A person having more Number_of_existing_loans_at_this_bank  and  Loan_history should have 
low chance of paying back loan

4. Tell us what your observations were on the data itself (completeness, skews).

The data had a lot of Non essential column, missing values and maximum categorical variables


TASK-2

File Named - ML model

Explain your intuition behind the features used for modeling.

I used  a decision tree because its  a flowchart-like structure in which each
internal node represents a "test" on an attribute (e.g.
whether a coin toss comes up heads or tails), each branch
represents the outcome of the test, and each leaf node
represents a class label (decision taken after computing all
attributes). It is useful  in cases where data set is very scaterred
in both X and Y axis in graph and in which multiple attributes are responsible for prediction





  

