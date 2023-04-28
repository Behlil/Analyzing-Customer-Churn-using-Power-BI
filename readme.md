
# Analyzing Customer Churn using Power BI

This project is about analyzing customer churn data using Power BI. The data contains information about customers who have left or stayed with a telecom company called Databel. The goal is to identify the patterns and factors that influence customer churn and provide insights for improving customer retention.

## Data Source

The data source for this project is a CSV file named databel.csv that contains 6687 rows and 25 columns. The columns include:

Metadata:

| Customer status | Description |
| --- | --- |
| Customer ID | The unique ID that identifies a customer |
| Churn Label | Contains “Yes” or “No” to indicate if a customer churned |
| Churn Reason | The particular reason why the customer ended the contract |
| Churn Category | Groups multiple churn reasons together for analysis purposes |


| Demographics | Description |
| --- | --- |
| Under 30 | Indicates if the customer is under 30 with “Yes” or “No” |
| Senior | Indicates if the customer is 65 or above with “Yes” or “No” |
| Age | The age of the customer |
| Gender | The gender of the customer, indicated by “Male”, “Female” or “Prefer not to say” |
| Group | Indicates if the customer is part of a group contract. A group contract offers advantages and is generally cheaper. Contains “Yes” or “No” |


| Contract information | Description |
| --- | --- |
| Number of customers in a group | Number of customers part of the group |
| Phone Number | Phone number of the customer |
| State | The code of the state where the customer lives |
| Payment Method | Preferred payment method of the customer indicated with “Credit Card”, “Direct Debit” or “Paper Check” |
| Contract Type | Contains “Month to Month”, “One Year” or “Two Year” |



| Subscription types & Charges | Description |
| --- | --- |
| Account Length (in months) | The number of months the customer has been with Databel |
| Local Calls | Amount of local (within the US) calls from the customer |
| Intl Calls | Amount of international (outside the US) calls from the customer |
| Intl Mins | The number of minutes spent calling internationally. |
| Intl Plan | Indicates if the customer has a premium plan to call internationally for free with “Yes” or “No”. This premium is reflected in the amount of the monthly charge |
| Extra International Charges | Additional charges incurred by the customer for making international calls without an international plan |
| Customer Service Calls | The number of times the customer contacted the customer service |
| Avg Monthly GB Download | The average amount of data downloaded by the customer per month in GB |
| Unlimited Data Plan | Indicates if the customer has an unlimited data plan with “Yes” or “No” |
| Extra Data Charges | Additional charges incurred by the customer for exceeding the data limit |
| Monthly Charges | The amount charged to the customer every month |
| Total Charges | The total amount charged to the customer for the entire duration of the contract |


## Data Preparation

The data was imported into Power BI and some transformations were applied using Power Query Editor. The transformations include:

- Changing the data types of some columns to match their values
- Replacing blank values with null values in total charges column
- Removing customer ID column as it is not relevant for analysis
- Creating a new column called group size based on the number of customers who have the same partner and dependents status
- Creating a new measure called churn rate based on the churn column

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

The project demonstrates how Power BI can be used to analyze customer churn data and provide valuable insights for improving customer retention.
