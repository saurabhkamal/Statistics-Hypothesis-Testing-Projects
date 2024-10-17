# International Soccer Matches, who scored more goals (Men Vs Women) - Wilcoxon-Mann-Whitney test

## Problem Statement

A major online sports media company, specializing in soccer analysis and reporting, wants to investigate that more goals are scored in women's international football matches than men's. This would make an interesting investigative article that their subscribers are bound to love; however this study aims to perform a valid statistical hypothesis test to be sure.

## Objective

The project's main goal is to run the Wilcoxon-Mann-Whitney test, a non-parametric test, if data is skewed or does not meet the assumption of normality required for a t-test. It would test whether women's matches tend to have higher goals scored than men's matches.

## Research Question

Are more goals scored in women's international soccer matches than men's?

Assuming a **10% significance level**, and the following null and alternative hypotheses:

$H_0$ : The mean number of goals scored in women's international soccer matches is the same as men's.

$H_A$ : The mean number of goals scored in women's international soccer matches is greater than men's.

## Determining Normality for Men's

![image](https://github.com/user-attachments/assets/4f0d83ea-260f-472c-a409-cc355e8e7724)

![image](https://github.com/user-attachments/assets/92427e14-2d4d-4ee6-9f36-2513d1c51c5e)

## Determining Normality for Women's

![image](https://github.com/user-attachments/assets/24ece1e6-3ad7-47a2-8611-b4ce132c8737)

![image](https://github.com/user-attachments/assets/df59c0da-dcb8-4360-8c94-af7d3cdbafb8)

**Goals scored is not normally distributed, so Wilcoxon-Mann-Whitney test of two group**

## Performing right-tailed Wilcoxon-Mann-Whitney test with pingouin

![image](https://github.com/user-attachments/assets/0ffc85c2-afc7-468f-8b48-858273f9a63d)

# Conclusion:

Since P-value < significance level, we have enough evidence to reject the null hypothesis. Hence, the goals scored in women's international matches is greater than men's
