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
- Null Hypothesis H(0): The Feature is independent of target column (No-Correlation)
- Alternative Hypothesis H(1): The Feature and Target column are not independent (Correlated)

## Univariate Analysis of Categorical Features
![image](https://github.com/user-attachments/assets/310e777a-9412-4d42-ba28-829ffd4ad744)

## **Insights**

From the uploaded **Univariate Analysis of Categorical Features** plots, you can infer the distribution of each categorical variable in your dataset. These visualizations give you insights into how different categories of each feature are represented. Here's a breakdown of what you can infer from each plot:

### 1. **Continent**:
   - The majority of the observations are from **Asia**, which dominates this category. Other continents like Africa, North America, Europe, South America, and Oceania have significantly fewer observations.
   - This suggests that most employees or applicants in your dataset are from Asia.

### 2. **Education of Employee**:
   - **Bachelor's** and **Master's** degrees make up the largest portions of the education level distribution, with fewer employees having a **High School** or **Doctorate** degree.
   - This indicates that the majority of individuals applying or in the dataset have relatively higher education levels (Bachelor's or Master's).

### 3. **Has Job Experience**:
   - A slightly larger proportion of employees **have job experience** (marked as "Y") compared to those without ("N").
   - This suggests that prior job experience is common among the employees or applicants in your data.

### 4. **Region of Employment**:
   - The **West**, **Northeast**, and **South** regions dominate the employment regions, while the **Midwest** and **Island** regions have relatively fewer entries.
   - This shows that the workforce or applicants are concentrated in these regions.

### 5. **Unit of Wage**:
   - The vast majority of the wages are given on a **yearly** basis, with very few instances of hourly, weekly, or monthly wage units.
   - This suggests that most employees or applicants are paid on an annual basis.

### 6. **Requires Job Training**:
   - Most employees do **not require job training** (N), and only a small portion requires it (Y).
   - This suggests that most of the jobs or applicants don’t need additional training.

### 7. **Full-time Position**:
   - Most of the positions are **full-time**, with very few part-time jobs represented in the dataset.
   - This indicates that the dataset is dominated by full-time positions.

### 8. **Case Status (Target Column)**:
   - A larger number of cases are **Certified** compared to those that are **Denied**.
   - This suggests that the majority of applications or cases in the dataset hgories in each feature are distributed.

## Chi-Square Test:

![image](https://github.com/user-attachments/assets/f7334ffa-aabc-4fd4-a28f-dc31b3572782)






