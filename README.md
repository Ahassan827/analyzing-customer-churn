# analyzing-customer-churn (Power bi)

## 📈Project Overview:

This project analyzes customer churn data to identify key factors and provide actionable insights for a telecommunications company. The analysis was conducted using a comprehensive Power BI dashboard, focusing on customer demographics, service usage, and payment behavior.




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


## Insight 1 — Pricing is the #1 Churn Driver :


The top stated reasons for churn were competitors offering better deals and prices being too high. Churn correlates directly with higher monthly charges, particularly among first-year customers.


So what? This is not just a pricing problem — it's a value perception problem. Customers aren't saying the service is bad; they're saying the price doesn't feel worth it. The fix is either adjusting price or better communicating value — not necessarily changing the product itself.
⚠️ Limitation: The largest single category in the churn reasons chart is N/A — meaning the majority of churned customers left without a recorded reason. The pricing insight is valid but represents only a subset of churned customers, not the full picture.



##  Insight 2 — Churn Behaves Differently Across Age Segments :


Young Customers (20–40): Churn is high in months 1–12, then drops sharply. These customers are testing the service — if they survive year one, they become loyal long-term customers.
Senior Customers (65+): Churn remains consistently high regardless of tenure. This is a chronic, ongoing issue likely tied to service complexity or inadequate support.


So what? These two segments need completely different solutions. One needs early intervention in the first year; the other needs a long-term structural fix in how support is delivered.



## Insight 3 — Monthly Contract + Direct Debit = Highest Risk Segment:


Customers on monthly contracts using Direct Debit show a 53.90% churn rate and higher-than-average service calls.


So what? This segment experiences ongoing friction — billing issues or unresolved complaints that accumulate until the customer decides to leave. This is the most actionable segment nationally because it is clearly identifiable and shows behavioral warning signals before churn actually happens.


## Insight 4 — Unlimited Data Plans are Misleading Moderate Users :


Customers on unlimited plans consuming 5–10 GB show a 33.57% churn rate — higher than heavy users who clearly get value from the plan.


So what? These customers are likely experiencing speed throttling or hidden limitations they did not expect from an "unlimited" plan. The issue is a trust gap, not a pricing gap. Greater transparency about plan limitations would likely reduce churn in this segment without any pricing change.


## Insight 5 — Group Plans are a Hidden Retention Tool :


Customers not on a group or family plan pay approximately double the monthly charge and show a churn rate nearly 3x higher compared to customers on group plans.


So what? Group plans are not just a pricing tier — they are one of the strongest retention mechanisms in the data. Customers with shared plans have lower charges per person and higher switching costs, making them significantly less likely to leave. Actively promoting group plan upgrades, especially to solo monthly contract customers, could simultaneously reduce churn and increase account value.


## Insight 6 — California Deep Dive :


California shows a 63.24% churn rate — 43 out of 68 customers lost. After filtering the dashboard specifically on California, three compounding problems were identified:


- Problem 1 — Monthly Contracts are an Open Exit Door:

Monthly + Paper Check = 100% churn

Monthly + Direct Debit = 94% churn

Monthly + Credit Card = 57% churn

Once a customer switches to a yearly contract, the numbers improve significantly across all payment methods.


- Problem 2 — International Charges are Burning Customers:

The average extra international charge in California is $36.19 on top of the base monthly bill. Given California's high demographic diversity and international activity, customers there are disproportionately affected by these additional costs compared to other states.


- Problem 3 — Customers Without Unlimited Data Leave Immediately:

Customers consuming 5–10 GB without an unlimited plan show a 100% churn rate in California. These customers are being surprised by unexpected extra data charges, which triggers an immediate decision to leave.


So what? California's problem is not a location-specific issue — it is a compounding combination of monthly contracts, unexpected billing, and uncompetitive international pricing. Competitors are present and ready to capitalize on every moment of customer frustration.




## 🛠️ Actionable Recommendations:

🔴 Priority 1 — California: Convert Monthly to Yearly Contracts (Quick Win)


The problem is clear and the solution is specific — the monthly contract is the primary driver of California's extreme churn rate.


Action: A targeted campaign for California's monthly contract customers offering a meaningful discount to switch to a yearly contract. In parallel, review international charge pricing specifically for the California market.




🟠 Priority 2 — Target Monthly/Direct Debit Segment Nationally


The same logic applies at a company-wide level — this segment has the highest churn rate and is the most identifiable and actionable group in the entire dataset.


Action: Proactive outreach campaign offering a clear incentive to switch from monthly to yearly contracts.
Estimated Impact: If 10% of this segment converts to yearly contracts, that is approximately 85 customers retained — and this is a conservative estimate based on available data.




🟡 Priority 3 — First-Year Engagement Program for Young Customers


High churn in months 1–12 is a known and consistent pattern. The solution is proactive, not reactive.


Action: Automated check-ins at 30, 60, and 90 days. A loyalty reward at the 6-month mark. Reinforce value before the customer starts comparing competitors.


🟢 Priority 4 — Fix Unlimited Plan Communication


No pricing change is needed here — only transparency.


Action: Clearly state data thresholds and speed policies in subscription materials and onboarding flows. Send in-app notifications when a customer approaches throttling limits.




🔵 Priority 5 — Senior Customer Dedicated Support Channel


This is the longest fix but addresses a persistent, structural problem that will not resolve itself.


Action: A dedicated support line for senior customers with simplified billing statements and clearer, more patient communication.




⚠️ Analysis Limitations


Churn Reasons Data Gap:
The largest category in the churn reasons chart is N/A — meaning the majority of customers who left did not have a recorded exit reason. This weakens confidence in some insights, particularly around pricing as the primary churn driver.
Recommendation: Implement a mandatory exit survey or cancellation flow that captures the churn reason before an account is closed. This single operational change would dramatically improve the quality of any future churn analysis.


<img width="1150" height="736" alt="1 1" src="https://github.com/user-attachments/assets/dc282bb7-4f1d-46e1-9e0f-16e1296611c3" />


<img width="1162" height="655" alt="1 2" src="https://github.com/user-attachments/assets/7f1157c8-5c26-46c8-acce-b6f9c90328a8" />


<img width="1167" height="657" alt="1 3" src="https://github.com/user-attachments/assets/e75af3cd-99d9-495a-8103-5ff4c3cd0ad7" />


<img width="1172" height="656" alt="1 4" src="https://github.com/user-attachments/assets/661de7d6-f68c-473d-a785-2bb02ddd3a53" />





