# Lending Club Case Study Project

## Problem Statement
'''Lending Club (LC) which is a marketplace for personal loans that matches borrowers who are seeking a loan with investors looking to lend money and make a return. When the company receives the loan application, it has to make a decision for loan approval based on applicant's profile.The company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.'''

## Table of Contents

* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information

###  Business Understanding

Consumer Finance company (Lending Club) is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface.

When a person applies for a loan, there are two types of decisions that could be taken by the company:

* 1. Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:

a. Fully paid: Applicant has fully paid the loan (the principal and the interest rate)

b. Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These
candidates are not labelled as 'defaulted'.

c.Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan

* 2. Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)

### Business Objectives

Lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.

If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.

###  Data Description

The dataset contains the complete loan data for all loans issued through the time period 2007 t0 2011 along with data dictionary for variable reference.


###  Data understanding
    - Understanding the data
###  Data Cleaning

    - Handling Missing values
    - Removal of single value columns
    - Data Imputation

###  Summary
    - Summary statistics for numeric attribute
    - Summary and value counts for Categorical attributes
### EDA 

#### Univariate analysis
    - Univariate Analysis for Continuous Variable
        * Boxplot ,histograms and distribution plots for all single variables
    - Univariate Analysis for Categorical Variable
        *countplot for all single categorical variable
        * pie plot for some combinations
#### Segmented Univariate analysis
#### Bivariate analysis
    - Box plot for all important numerical variables with loan_status¶
    - Box plot for all important numerical variables with grade¶
    - Bar Plot for all important numerical variables with dti ratio¶
    - Barplot for all the imporatant categorical variables with loan amount
    - Bar plot for all the important categorical variables with annual income¶
    - Bar plot for all the important categorical variables with Loan_amount
#### Multivariate analysis
    - Multivariate analysis between home_ownership,annual_inc_cat,loan_status and issue_year
    - Multivariate analysis between dti,annual_inc_cat,loan_status and term¶
    - Multivariate analysis between purpose,loan_amnt,loan_status and term
    - Correlation among the numeric variables.
 
## Conclusion

1. The income source should be verified thoroughly before sanctioning the loan.
2. People who are having low annual salary and high dti ratio are more likely to be defaulter.
3. It is risky to give big loan amount to applicants with higher dti.
4. Small loan amounts are always non risky.
5. Large loan amount for small business should not have the home ownership as mortgaged.
6. People with higher dti meaning that their monthly income mostly goes to pay their debts. These debts are higher for the people who have taken loan to repay their credit card bills and Such people are likely to default a loan. On the other hand,the people with dti between 10-12 are less likely to default as they have taken loan for educational or house purpose.

## Technologies Used
- Jupyter Notbook (anaconda3)
- Python Language
- pandas library 1.4.1
- numpy library 1.22.2
- seaborn library 0.11.2
- matplotlib library 3.5.1


## Acknowledgements

Thanks for Upgrad to give this case study to learn. This is very inspiring project to learn many tools and techniques to analyze the data and draw the insights.

#### References: 

Referred some sites for some business terminologies:
https://www.nationalfunding.com/blog/what-is-revolving-utilization-how-to-improve-it/
https://www.experian.com/blogs/ask-experian/credit-education/score-basics/credit-utilization-rate/
https://www.capitalone.com/learn-grow/money-management/revolving-credit-balance/
https://www.investopedia.com/terms/d/dti.asp
https://www.investopedia.com/terms/c/credit-inquiry.asp
https://www.investopedia.com/terms/a/average-outstanding-balance.asp

- This project was based on (https://www.lendingclub.com/).

## Contributors

Created by,
  -Prathima Kumari B V
  -Seema Simoliya

Developed as part of the Exloratory Data Analysis Module required for Advanced Certificate Program for ML and AI - IIIT,Bangalore.
