# TELECOM-CUSTOMER-CHURN-ANALYSIS
This project is designed to transition the company's retention strategy from reactive recovery to proactive, data-driven defense. The primary aim is to minimize attrition and maximize Customer Lifetime Value (CLV) by focusing on the highest-risk, highest-value segments.

## Project Objectives:
• Financial Objective: Reduce the 16% Churn Rate to protect the $61.78K in Annual Revenue at Risk.

• Operational Objective: Prioritize fixing the 20+ Call Failure service threshold, the operational trigger causing significant churn spikes.

• Targeted Objective: Increase the retention rate of the financially-critical 'High Value - Low Engagement' segment.

• Commitment Objective: Implement early-life campaigns to secure contract commitment from the high-volume 'New - High Risk' segment.

• Behavioral Objective: Increase customer service usage (e.g., Frequency of Use) by 15% for high-risk customers to boost loyalty

## Data Used
-	<a href="https://github.com/Bolatito12/TELECOM-CUSTOMER-CHURN-ANALYSIS/blob/main/customer_churn%20(2).csv">Dataset</a>
-	<a href="https://github.com/Bolatito12/TELECOM-CUSTOMER-CHURN-ANALYSIS/blob/main/feature_importance%20(1).xlsx">Dataset</a>

##  Key Problems & Questions
1. What is the overall churn rate among telecom customers?
2. Which customer segments show the highest churn risk?
3. How does churn vary by plan type or subscription level?
4. What is the relationship between usage patterns and churn?
5. How does customer tenure affect churn likelihood?
6. Can we identify early warning signals of churn from customer activity?

## Exploratory Data Analysis (EDA) 
#Import Libraries
<img width="1837" height="318" alt="python code1" src="https://github.com/user-attachments/assets/d47f1a9a-a33c-4e47-8e81-7476563824d3" />

#Read file
<img width="1765" height="172" alt="python code 2" src="https://github.com/user-attachments/assets/696128a1-29ed-4972-bf65-2c349f94d4ed" />

#Check number of row and column and also datatype
<img width="1719" height="363" alt="python code 3" src="https://github.com/user-attachments/assets/471ee3e9-a7ef-4420-af43-1f01a78b8ca0" />

#check for missing values and duplicates
<img width="1920" height="587" alt="python code 4" src="https://github.com/user-attachments/assets/d437cc40-4683-4bfd-bbcf-d48931529717" />

## Univariate Analysis (Target + All Features)

Goal:
Understand the distribution and behavior of each variable independently to identify patterns, imbalance, and potential data issues.

## Target Variable: Churn

Insights:

• The dataset shows an imbalance between churned and non-churned customers, with a larger proportion of customers retained.

## Numeric Variables

Variables Analyzed:
• Call Failure, Subscription Length, Charge Amount, Seconds of Use, Frequency of Use, Frequency of SMS, Distinct Called Numbers, Customer Value, Age

Insights:

• Most numeric variables are right-skewed, indicating that a small number of customers have very high usage or value.

• Subscription Length is concentrated at lower values, suggesting many customers churn early in their lifecycle.

• Charge Amount and Customer Value show high variability, indicating heterogeneous customer spending behavior.

<img width="1218" height="913" alt="image" src="https://github.com/user-attachments/assets/f781a459-5b76-476b-be38-87ca1467ada0" />


## Categorical / Ordinal Variables

Variables Analyzed:
• Complaints, Tariff Plan, Status, Age Group

Insights:

• The majority of customers fall into a small number of tariff plans, suggesting limited plan diversity.

• Customers without complaints form the largest group, while a smaller but important segment has registered complaints.

• Age Group distribution shows a higher concentration of customers in middle-aged groups, with fewer elderly customers.

## Bivariate Analysis (Feature vs Target)

Goal:
Identify which customer attributes are associated with higher churn risk and understand their influence on customer attrition.

## Numeric Variables vs Churn

Insights:

• Churned customers tend to have shorter subscription lengths, confirming that early-stage customers are more likely to leave.

• Higher call failure rates are associated with increased churn, highlighting the impact of service quality issues.

• Customers with lower seconds of use and lower frequency of use are more likely to churn, suggesting disengagement.

• Higher charge amounts are linked to higher churn, indicating potential price sensitivity.

• Customer Value is generally lower among churned customers, suggesting churn is more common among less valuable customers.

• Age shows a mild relationship with churn, with younger customers slightly more likely to churn.

## Categorical Variables vs Churn

Insights:

• Customers who have filed complaints exhibit significantly higher churn rates than those without complaints.

• Certain tariff plans show noticeably higher churn, suggesting pricing or plan structure issues.

• Inactive or suspended customer status is strongly associated with churn.

• Younger age groups demonstrate higher churn rates compared to older groups, indicating lower loyalty.

## Predictive model for feature importance 
<img width="923" height="690" alt="python code 6" src="https://github.com/user-attachments/assets/512fc3af-a548-4892-bb71-0fff61486b82" />

