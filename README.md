# analyzing-customer-churn (Power bi)

## 📈Project Overview:

This project analyzes customer churn data to identify key factors and provide actionable insights for a telecommunications company. The analysis was conducted using a comprehensive Power BI dashboard, focusing on customer demographics, service usage, and payment behavior.

## 🚀 The Big Picture:

Our Key Performance Indicators
Before the analysis, let's look at the numbers. They tell a story of a company with a significant retention challenge.



# 📊 Dataset Overview

- Number of rows : 6687
- Number of columns: 29
- Data Source: Datacamp
- Key Columns: customer ID , Gender , Age , Contract Type , Payment Method , Monthly Charges, Total Charge , Churn

---

## 🧹 Data Cleaning (Power Query)
- Filled missing values with **"N/A"**  
- Removed duplicates  
- Standardized data types (numeric, categorical, date)   

---

## 📏 Measures

| Measure                          | Description                                    |
|----------------------------------|------------------------------------------------|
| Avg Customer Service Calls       | Average number of service calls per customer   |
| Avg Extra Data Charges           | Average additional data charges per customer   |
| Avg Extra International Charges  | Average international charges per customer     |
| Churn Rate %                     | % of churned customers                        |
| Number Of Churned Customers      | Total churned customers                       |
| Number Of Customers              | Total customers (based on filters)            |
| Number Of Unique Customers       | Distinct count of customers                   |

---

## 📂 Added Columns

| Column              |  Purpose                                  |
|---------------------|-------------------------------------------|
| Churned             |  Indicates if customer churned (1,0)      |
| Contract category   |  Contract type (Monthly, Yearly)          |
| Demographics        | Age  ( Under 30 , Senior , Other          |
| Group consumption   | Usage/consumption in group or family plan |
| Age bins            | Age grouped into ranges for analysis      |



---

## 🎯 KPI	

. Total Customers	6,687	

. Churned Customers	1,796

. Overall Churn Rate	26.86%

. Avg. Customer Service Calls	0.92	

. Avg. Extra International Charges	$33.64


---

## 🔍 Key Insights from the Analysis:

A deep-dive into the data revealed several critical insights into customer behavior and churn drivers.

1. Pricing and Value Proposition are the Primary Churn Drivers:

The top two reasons for churn were identified as "Competitor made a better offer" and "Price too high".

Churn is directly correlated with higher monthly charges, especially for new customers.

This indicates a gap in the company's value proposition and competitive pricing.

2. Churn is Segment-Specific and Varies with Customer Tenure:

New Customers (Age 20-40): This segment shows a high churn rate in their first year (1-12 months), but their loyalty increases significantly afterward, with churn dropping to near zero for long-term customers.

Senior Customers (Age 65+): This group exhibits a consistently high churn rate across all account tenures, suggesting a persistent, long-term issue related to service complexity or support.

3. Contract Type and Payment Method are Critical Indicators of Churn:

Monthly contracts have a significantly higher churn rate compared to yearly contracts.

Customers on monthly contracts using Direct Debit are the most at-risk segment, showing a churn rate of 53.90% and higher average customer service calls, pointing to potential billing or service issues.

4. Data Plan Performance is a Hidden Churn Factor:

A high churn rate of 33.57% was observed among customers with an "unlimited data plan" who consume a moderate amount of data (5-10 GB).

This suggests a potential disconnect between the perceived value of the "unlimited" plan and the actual service delivered (e.g., speed throttling, hidden limitations), leading to customer frustration.

5- Geographical Insight

California (CA) shows the highest churn rate among all states.

Interestingly, CA also records the lowest average customer service interaction rate, suggesting low engagement or dissatisfaction resolution, which may be intensifying churn in this region.



---

## 🛠️ Actionable Recommendations:

From Insights to Impact
Here’s a strategic roadmap to turn these insights into business results.

💰 Re-evaluate Pricing & Value:

Conduct a competitive price analysis.

Create targeted promotions to make our offers more attractive, especially for new customers.

🛡️ Protect Our Most At-Risk Customers:

For New & Young Customers: Launch a "First-Year Engagement" program to proactively check on satisfaction and reinforce our value.

For Senior Customers: Develop a specialized, simplified support channel and offer clearer billing statements to solve their ongoing challenges.

🤝 Incentivize Loyalty:

Offer significant discounts or perks to encourage customers to switch from monthly to more stable, yearly contracts.

Be transparent about the true value and any limitations of "unlimited" data plans to build trust and manage expectations.

🌍 Localize Our Strategy

Prioritize California by implementing local retention initiatives, improving customer support accessibility, and increasing communication touchpoints.

Continue to use geographical analysis to identify and resolve region-specific issues in other high-churn areas.



<img width="1150" height="736" alt="1 1" src="https://github.com/user-attachments/assets/dc282bb7-4f1d-46e1-9e0f-16e1296611c3" />


<img width="1162" height="655" alt="1 2" src="https://github.com/user-attachments/assets/7f1157c8-5c26-46c8-acce-b6f9c90328a8" />


<img width="1167" height="657" alt="1 3" src="https://github.com/user-attachments/assets/e75af3cd-99d9-495a-8103-5ff4c3cd0ad7" />


<img width="1172" height="656" alt="1 4" src="https://github.com/user-attachments/assets/661de7d6-f68c-473d-a785-2bb02ddd3a53" />





