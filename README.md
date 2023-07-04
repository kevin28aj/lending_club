# LendingClub EDA

Develop recommendations to predict ability to repay loans based on applicant's profile when the company receives a loan application. We will focus on defining the driving factors behind loan default, so that the company can use this data to perform risk assessment.

## Table of Contents
* [General Info](#general-information)
* [Data Analysis & Cleanup](#data-analysis--cleanup)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

## General Information
- LendingClub provides loans of various types to urban customers, when the company receives an application it has to make a decision based on applicant's risk profile. Basically there are two risks, i.e
    - Applicant is likely to repay, but application not approved leading to loss of business.
    - Applicant is not likely to repay, but application is approved, leading to financial loss.
- This project will focus on identifying key driver variables that will help determine an applicant's ability to repay the loan.
- Dataset has information about past loan applicant's whether they defaulter or not, we will use this information to identify pattern which will indicate if an applicant is likely to default or not.

## Data Analysis & Cleanup:
    - Dataset has lot of missing values
        - All columns that has more than 90% missing values has been removed.
        - All rows with more than 25% missing values has been removed.
    - Impute Variables
        - emp_length variable need to be imputed.
    - Target Variables
        - loan_default_status variable has been created as boolean to aggregate and plot status.
    - Driver Variables
        - grade, purpose, emp_length, home_ownership, application_type, addr_state

## Conclusions
- An applicant is more likely to default loan re-payment, when type of residence is Rented or Mortgaged when compared to Owned.
- An applicant is more likely to default loan re-payment, when purpose of loan is for debt consolidation as opposed to any other purpose.
- Applicant's that has worked at an employer for longer term, i.e. 10+ years tend to re-pay better.
- Applicants belonging to E,F,G grades are more likely to default on loan re-payment.
- Applicants from state of California has higher changes of a loan default than most other states.

## Technologies Used
- python 3
- jupyter notebook

## Contact
Created by [@kevin28aj]!