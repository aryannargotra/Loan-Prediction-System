# Loan-Prediction-System
Data Science Assignment - REUNION


File named Data Insights

Task 1

1. Do the Exploratory Data Analysis & share the insights.

  Firstly read both csv files and did the exploratory analysis of both checked the relationship 
  between the Number of existing loans at this bank with High Risk applicant and bivariate         analysis of Principal_loan_amount and Balance_in_existing_bank_account_(lower_limit_of_bucket)


2. How would you segment customers based on their risk (of default)?

    Merged the Applicant and Loan dataframes then removed the non essential columns merged           
    Applicant Id and High risk applicant column in same table ordered by their risk.

3. Which of these segments / sub-segments would you propose be approved?

    A person having more Number_of_existing_loans_at_this_bank  and  Loan_history should have 
    low chance of paying back loan

4. Tell us what your observations were on the data itself (completeness, skews).

    The data had a lot of Non essential column, missing values and maximum categorical variables


TASK-2

File Named - ML model

1 . Explain your intuition behind the features used for modeling.Are you creating new derived        features? If yes explain the intuition behind them

  I used  a decision tree because its  a flowchart-like structure in which each
  internal node represents a "test" on an attribute (e.g.
  whether a coin toss comes up heads or tails), each branch
  represents the outcome of the test, and each leaf node
  represents a class label (decision taken after computing all
  attributes). It is useful  in cases where data set is very scaterred
  in both X and Y axis in graph and in which multiple attributes are responsible for             prediction. After that I used GaussianNB because It is easy and fast to predict the class of   the test data set. It also performs well in multi-class prediction. And finally a Logistic     regression
  
2. Are there missing values? If yes how you plan to handle it.

   Yes there were missing values I handled it by using  Pandas methods help us achieve this in    a single line of code for every column. The fillna()method fills the empty fields with        whatever parameter is given.Calculating the mean or mode of this array of values, and          passing it to fillna() completes this step.Using mode works best in our case, as most          columns are binary. Moreover, Mode will simply put the most occurring instance in place of    empty fields, which, under the circumstances, would be the best guess. 
   
   
3.  How categorical features are handled for modeling.
    
    Using use the get_dummies function of Pandas for non-binary values like 'Property' to         automatically one-hot encode them
    
4. Describe the features correlation using correlation matrix. Tell us about few correlated      feature & share your understanding on why they are correlated.

   A correlation matrix is a table showing the correlation coefficients between different sets    of variables  
   
   I've used seaborn heatmap for correlation in which the red/warm color denotes the stronger
   corelation and in our dataframe Principal_loan_amount and months_loan_taken for a strong 
   corelation because if the we increase loan amount the duration of loan also increases and 
   Emi rate and loan amount have inverse corelation
   
  5. Do you plan to drop the correlated feature? If yes then how.

     Yes I plan to showcase this feature using Seaborn heatmap because coolwarm colors really 
     makes it easy to identify the correlation in dataframe.
     
 6.  Which ML algorithm you plan to use for modeling. and Their different parameters

     I used  a decision tree because its useful us in cases where data set is very scaterred
     in both X and Y axis in graphs. It gave a accuracy of 64%
     
     
     After That I used GaussianNB It perform well in case of categorical input variables            compared to numerical variable. I performed it to compare it with the Logistic Regression
     and see the difference between the accuracy 
     
     Finally I used the Logistic Regression because it works well with bonary numeric values 
     since after normalising most of the values in numeric binary Logistic regression gave us      the best accurancy of 72%.
     
  7.   Explain how you will export the trained models & deploy it for prediction in                  production.
     
       We can use TensorFlow model creation then create webservice to serve the client request
       create deployment container with webservice, test the container, put it in production
    
     
     
     
     

     
     
     
   
   
   







  

