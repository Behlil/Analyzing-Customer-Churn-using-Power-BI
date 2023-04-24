
# Analyzing Customer Churn using Power BI

This project is about analyzing customer churn data using Power BI. The data contains information about customers who have left or stayed with a telecom company. The goal is to identify the patterns and factors that influence customer churn and provide insights for improving customer retention.

## Data Source

The data source for this project is a CSV file that contains 7043 rows and 21 columns. The columns include customer ID, gender, senior citizen, partner, dependents, tenure, phone service, multiple lines, internet service, online security, online backup, device protection, tech support, streaming TV, streaming movies, contract, paperless billing, payment method, monthly charges, total charges and churn.

The data was obtained from [Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn).

## Data Preparation

The data was imported into Power BI and some transformations were applied using Power Query Editor. The transformations include:

- Changing the data types of some columns to match their values
- Replacing blank values with null values in total charges column
- Removing customer ID column as it is not relevant for analysis
- Creating a new column called group size based on the number of customers who have the same partner and dependents status
- Creating a new column called international plan based on the phone service and multiple lines columns
- Creating a new column called churn rate based on the churn column

## Data Analysis

The data analysis was done using Power BI Desktop and Power BI Service. The analysis includes:

- Creating various measures and calculated columns using DAX formulas
- Creating various charts and tables to visualize the data and explore the relationships between different variables
- Creating a dashboard and a report to summarize the findings and insights

## Churn Patterns

The analysis revealed some interesting patterns and insights about customer churn. Some of them are:

- Churn rate is about 27%.
- Competition is the main churn reason with 44%.
- California has the biggest churn rate: more than 60%.
- Senior citizens are more likely to have churn rate: 38%.
- In general, the churn rate has an increasing trend through the age brackets.
- As the Age increases, the average churn rate for age brackets also increase.
- Group with 6 Customers has the lowest churn rate.
- Monthly Charges is significantly lower for people who are in a group of 2 or more.
- Customers who have monthly contracts churn more than customers who have yearly-based contacts.
- Customers who are on an unlimited plan are more likely to churn.
- When considering only the State with the highest churn rate(California), 72% of customers who actively make international calls but do not have an international plan churn
- 100% of customers who have an international plan but are not using it churn.
- New Customers are more likely to churn. The churn rate decrease over time.
- Only a small group of 371 customers who uses Paper Check as a payment method.

## Conclusion

The project demonstrates how Power BI can be used to analyze customer churn data and provide valuable insights for improving customer retention. The project also shows how to write a good readme file for GitHub using Markdown syntax and best practices.

