## Problem Statement: 
In the rapidly evolving taxi booking industry, optimizing revenue is crucial for sustained success and driver satisfaction. Our objective is to leverage data-driven insights to enhance revenue opportunities for taxi drivers. This study aims to explore the impact of payment methods on fare pricing, focusing on the connection between payment type and fare amount.

## Research Question
Is there a connection between payment type and total fare amount, and can we encourage customers to choose payment methods that boost driver revenue without compromising their overall experience?

## Data Overview
For this analysis, we leveraged the extensive NYC Taxi Trip Records dataset, applying data cleaning and feature engineering techniques to focus only on the key columns relevant to our study.

### Relevant columns used for this research
- passenger_count (1 to 5)
- payment_type (card or cash)
- fare_amount
- trip_distance (miles)
- duration (minutes)

## Methodology
- **Descriptive Analysis**: Conducted statistical analysis to highlight important features of the data, with an emphasis on fare amounts and payment methods.
- **Hypothesis Testing**: Performed a T-test to assess the link between payment method and fare amount, examining the hypothesis that various payment types affect fare amounts.

## Journey Insights
- Customers who pay by card generally have a slightly higher average trip distance and fare amount compared to those paying with cash.
- This suggests that customers tend to use cards for longer trips and higher fare amounts.

![image](https://github.com/user-attachments/assets/2b0d8204-865b-4faa-afa2-920a3bd93e27)

![image](https://github.com/user-attachments/assets/63cf31cb-aa3d-4c94-8810-79d5e2868d13)


## Preference of Payment Types
- A significantly larger proportion of customers pay with cards than with cash, with card payments making up 67.5% of all transactions, while cash payments account for 32.5%.
- This suggests a clear customer preference for card payments over cash, likely driven by factors such as convenience, security, or rewards associated with card transactions.

![image](https://github.com/user-attachments/assets/24f028b7-1a8a-4189-86c9-5352572a6bff)


## Passenger Count Analysis
- Single-passenger rides (passenger_count=1) make up the largest share of card payments, accounting for 40.08% of all card transactions.
- Likewise, cash payments are primarily linked to single-passenger rides, representing 20.04% of all cash transactions.
- These insights highlight the significance of factoring in both payment method and passenger count when analyzing transaction data, as they offer valuable perspectives on customer behavior and preferences.

![image](https://github.com/user-attachments/assets/dcd57d5f-78ba-4699-a984-dfdec753e79d)

## Hypothesis Testing
**Null Hypothesis (H0):** There is no difference in the average fare between customers who pay with credit cards and those who pay with cash.

**Alternate Hypothesis (H1):** There is a difference in the average fare between customers who pay with credit cards and those who pay with cash.

With a T-Statistic of 165.5 and a P-value below 0.05, we reject the null hypothesis, indicating that there is a significant difference in average fare between the two payment methods.

## Recommendations
1. Motivate customers to use credit cards to take advantage of the potential for increased revenue for taxi drivers.  
2. Introduce strategies like offering incentives or discounts for credit card payments to encourage customers to select this payment method.  
3. Offer smooth and secure credit card payment options to improve customer convenience and promote the use of this preferred payment method.  
  
