# Retail-Customer-Retention-Analytics

Project Summary

Walmart operates at massive scale across physical stores and e-commerce. The real problem is not data availability, it’s poor analytical depth. This project fixes that.

The goal is to build a Customer Retention Analytics Dashboard in Power BI that helps Walmart:

Understand why customers churn

Identify loyal vs at-risk customers

Measure loyalty programs and promotions impact

Drive region- and channel-specific retention strategies

This is decision support, not a vanity dashboard.

🎯 Business Problem

Customer acquisition is expensive. Retention is cheaper and smarter.

Walmart’s existing reporting answers what happened, not:

Who is likely to churn?

Which customers are worth saving?

Which loyalty tiers and channels actually work?

This project directly addresses those gaps.

🧠 Project Objectives

The Power BI dashboard is designed to:

Consolidate fragmented customer, transaction, loyalty, and churn data

Enable dynamic segmentation (churned, repeat, high-value customers)

Track churn, repeat behavior, promotions, loyalty effectiveness, and CLV

Deliver actionable insights, not generic charts

📂 Dataset Overview
1. Customer_Demographics.csv
Column	Description
Customer_ID	Unique customer identifier
Age, Gender	Customer profile
Region	Geographic region
Income_Level	Income category
Membership_Since	Loyalty start date
Preferred_Channel	Store / Online
2. Customer_Transactions.csv
Column	Description
Transaction_ID	Unique transaction
Customer_ID	Linked customer
Store_ID	Store identifier
Product_Category	Product type
Transaction_Date	Date of purchase
Amount	Purchase value
Promotion_Applied	Yes / No
3. Store_Locations.csv
Column	Description
Store_ID	Store identifier
Store_Type	Supercenter / Online etc.
Region	Store region
Opening_Year	Year opened
4. Loyalty_Program.csv
Column	Description
Customer_ID	Customer identifier
Loyalty_Tier	Basic → Elite
Points_Earned	Loyalty points
Points_Redeemed	Points used
5. Churn_Labelled_Customers.csv
Column	Description
Customer_ID	Customer identifier
Last_Purchase_Date	Last activity
Churn_Flag	0 = Active, 1 = Churned
Churn_Reason	Reason for churn
🛠️ Tools & Technologies

Power BI Desktop

Power Query (Data cleaning & transformation)

DAX (KPIs, CLV, churn metrics)

Excel / CSV datasets

No AI-generated analysis was used for task execution.

🔗 Data Model

One-to-Many

Customer_Demographics → Transactions

Customer_Demographics → Loyalty_Program

Customer_Demographics → Churn_Labelled_Customers

Many-to-One

Transactions → Store_Locations

This ensures clean filtering and accurate KPIs.
