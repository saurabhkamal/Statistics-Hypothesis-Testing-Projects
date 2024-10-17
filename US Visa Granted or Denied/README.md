# US Visa Granted or Denied (Chi-Square Test)

## About
The Immigration and Nationality Act (INA) of the US permits foreign workers to come to the United States to work on either a temporary or permanent basis. The act also protects US workers against adverse impacts on working place and maintain requirements when they hire foreign workers to fill workforce shortages. The immigration programs are administered by the Office of Foreign Labor Certification (OFLC).

## Problem statement
- OFLC gives job certification applications for employers seeking to bring foreign workers into the United States and grants certifications.
- As in last year the count of employees was huge and OFLC wants to analyze important variables that can determine whether to grant or deny job certification applications.

## Objective
This project's main goal is to run a Chi-square test of independence to examine the relationship between categorical features and case status, the target variable. We use Python hypothesis testing and other analyses to extract useful information that can help OFLC grant or deny job certification applications. In particular, we want to test the correlation of Categorical columns with Target column

## Research Question
Is there a connection between continent, education_of_employee, has_job_experience, requires_job_training, region_of_employment, unit_of_wage, and full_time_position, and case_status since correlated features can help in prediction. Features that have some level of correlation or relationship with the target variable are generally more useful for prediction. If there is no relationship, the model may not perform well because the features won't provide helpful information to predict the target?

## Relevant columns used for this research
- continent  
- education_of_employee 
- has_job_experience 
- requires_job_training 
- region_of_employment 
- unit_of_wage 
- full_time_position
- case_status

## Methodology
**- Hypothesis Testing:** Performed Chi-Square test to assess the correlation between categorical columns and target column and determining whether to reject or fail to reject the null hypothesis

## Hypothesis Testing:
- Null Hypothesis ($ H_0 $): The Feature is independent of target column (No-Correlation)
- Alternative Hypothesis ($ H_1 $): The Feature and Target column are not independent (Correlated)


