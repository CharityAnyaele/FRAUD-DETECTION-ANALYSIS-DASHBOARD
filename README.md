# FRAUD-DETECTION-ANALYSIS-DASHBOARD
I created a Power BI dashboard designed to analyze fraudulent transactions within the dataset. The report provides interactive visuals and key performance indicators (KPIs) to identify patterns, track fraudulent activities, and explore transaction behaviors across multiple dimensions.
## Project Objectives:
The main goal of this project was to design a Power BI dashboard that provides clear insights into fraudulent transactions within a dataset. Specifically, the objectives were:
	•	To identify and quantify fraudulent activities.
	•	To create key performance indicators (KPIs) that summarize the scale of fraud. 
	•	To explore fraud patterns across multiple dimensions (e.g., city, payment method, device used).
	•	To build an interactive dashboard that allows users to filter and drill down into details for further investigation.
	## Data Used
	front-<a href="https://github.com/CharityAnyaele/FRAUD-DETECTION-ANALYSIS-DASHBOARD/blob/main/FRAUD%20DETECTION%20ANALYSIS.pbix">Dataset</a>
	##2. Data Description

The dataset contained the following key columns:
	•	Fraud amount – the monetary value of fraudulent activity.
	•	Transaction id – unique identifier for each transaction.
	•	Payment method – the method used (e.g., card, transfer, etc.).
	•	City – location of the transaction.
	•	Device used – device type (desktop, mobile, etc.).
	•	Account age – how long the account has existed.
	•	Number of times transactions – frequency of transactions by a user.
	•	Transaction type – category of transaction.
	## Dataset tools used for this project
	
 3. Tools & Technologies
    . Excel for cleaning the data
	•	Microsoft Power BI → used for building the dashboard, visualizing data, and creating interactive reports.
	•	Power Query → used also for minimal data cleaning and transformations (ensuring fraud amounts and transaction details were ready for analysis).
	•	DAX (Data Analysis Expressions) → used for creating custom measures, including:
	•	Fraudulent Transactions 
	•	Fraud Rate %
    . Total fraud transaction. 
    ## Steps taken on this project;

      Methodology
	1.	Data Preparation
	•	Loaded the dataset from Excel into Power BI.
	•	Cleaned the data using Power Query (checked nulls, corrected column formats).
	•	Ensured fraud amounts were numerical and could be aggregated.
	2.	Measure Creation (DAX)
	•	Built measures to calculate KPIs like Total Fraud Amount and total transactions.
	•	Used calculated fields to update values when filters are applied dynamically.
     ## Detailed formulas used:
    1. I used Excel to separate my data by using ('TEXT to columns' to separate each column, and used the 'PROPER' function to capitalize my City name and transaction type            column.
    2. For other data cleaning, I used Power Query by selecting my table, where I removed duplicates, used TRIM text (to remove extra spaces, and changed data types to           numbers, text, and dates.
    3. I created a new column and categorized the Account age using the IF FUNCTION for example; =IF(I2<25, "New account"), IF(I2<=35, "Young account"), IF(I2<=45, "Established account"), IF(I2<=55, "Mature account"), IF(I2>56, "Old account")
    4. I got the sum of the previous fraud transaction and the current fraud transaction of each offender by using the equation e.g = H2+L2
    5. To confirm my total completed transactions were correct, I use DAX Query, for example, Total Completed transactions = SUM(TransactionData [Completed transactions])
    6. I created my dashboard and a slicer to filter data information of the payment methods like credit card, debit card, Net banking, and UPI.
       
    
   	
		## Dashboard Development
	•	Placed 2 key KPIs at the top for quick insight:
	•	Total Transactions
	•	Total Fraud Amount
	•	Fraud Rate (%)
	•	Created supporting visuals:
	•	Fraud by Payment Method
	•	Fraud by City
	•	Fraud by Device Used
	•	Fraud by Account Age
     ##  Final results 

 5. Results & Insights

The completed dashboard provided both summary KPIs and detailed breakdowns:
	•	Fraud Rate (%) → showed total transactions were fraudulent.
	•	Dimensional Analysis → helped identify where fraud was most prevalent:
	•	Certain payment methods showed higher fraud concentration.
	•	Fraud activity varied across cities and devices.
	•	Older accounts tended to have higher fraud rates compared to Newer accounts.
	.    Total completed transactions.

## Conclusion

This project successfully demonstrated how Power BI can be used for fraud detection analysis. The dashboard provides an accessible way to monitor fraudulent activities, summarize KPIs, and drill into details across different dimensions. With further development, this approach can be extended to include predictive analytics (machine learning models for fraud detection) and real-time monitoring using live data sources.
## FINAL DASHBOARD 
![FRAUD ANALYSIS DASHBOARD](https://github.com/user-attachments/assets/84b83fbf-6ddf-4486-b00f-5478301ce820)





