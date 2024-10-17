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

![image](https://github.com/user-attachments/assets/44734055-1eb4-4ab5-afb7-132a47119046)

#### **Report**

The table summarizes the results of Chi-square tests conducted on various categorical features in relation to the target variable, `case_status`. 

### Table Explanation

1. **Columns**:
   - **Column**: This refers to the categorical feature that was tested for independence with the target variable `case_status`.
   - **Hypothesis Result**: This shows the outcome of the Chi-square test for each feature concerning the null hypothesis.

2. **Results**:
   - **Reject Null Hypothesis**: This outcome suggests that there is a statistically significant association between the feature and the target variable (`case_status`). In other words, the distribution of the target variable varies depending on the category of the feature.
   - **Fail to Reject Null Hypothesis**: This means there is no statistically significant evidence to suggest an association between the feature and the target variable. The feature does not significantly influence or relate to the distribution of the target variable.

### Interpretation of Each Row

- **`continent`**: The result indicates a significant relationship between `continent` and `case_status`, meaning that the status (Denied or Certified) is likely dependent on the continent from which the individual is.
  
- **`education_of_employee`**: Similar to `continent`, this feature shows a significant association with the target variable, suggesting that educational background may influence the outcome of `case_status`.

- **`has_job_experience`**: This feature also shows a significant relationship, indicating that whether an individual has job experience could affect their `case_status`.

- **`requires_job_training`**: The result shows "Fail to Reject Null Hypothesis," indicating no significant association with `case_status`. This suggests that the requirement for job training does not meaningfully affect the outcome.

- **`region_of_employment`**: This feature is significant, suggesting that the region where an individual is employed may influence their `case_status`.

- **`unit_of_wage`**: This feature also indicates a significant relationship with the `case_status`, implying that how wages are calculated might affect the outcome.

- **`full_time_position`**: The outcome here suggests a significant association, meaning whether an employee is in a full-time position can influence their `case_status`.

- **`case_status`**: While it may seem redundant to include `case_status` in this context, its inclusion here confirms that the variable is indeed significant to itself (which is a logical requirement).

### Overall Conclusion

The overall results suggest that several categorical features are significantly associated with the `case_status`, while only `requires_job_training` does not show a significant relationship. 

This implies that when predicting or analyzing `case_status`, the features `continent`, `education_of_employee`, `has_job_experience`, `region_of_employment`, `unit_of_wage`, and `full_time_position` should be considered as they might have a meaningful impact on the outcome. The results of this Chi-square test can guide further analysis and modeling efforts, as it highlights features worth focusing on for understandiation on any part, feel free to ask!




