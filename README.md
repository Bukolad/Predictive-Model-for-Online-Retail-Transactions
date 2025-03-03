# Retail Sales Analysis and Forecast
## Project Overview
This project aims to develop a predictive model that classifies online retail transactions into specific categories and clusters. The model helps uncover hidden patterns in customer segmentation, optimize inventory management, and enhance sales forecasting.
## Objectives
- Customer Segmentation: Identify different customer groups based on purchasing behavior.
- Inventory Optimization: Predict demand for products and manage stock efficiently.
- Sales Forecasting: Analyze trends to make data-driven sales predictions.
## Datasets Column
- InvoiceNo
- StockCode	
- Description	
- Quantity	
- InvoiceDate	
- UnitPrice	
- CustomerID	
- Country
## Issues Identified
- 1,454 missing values in Description(Products)
- 10,624 negative values in Quantity
- 135,080 missing values in CustomerID
- 5,226 Duplicate Values
- Invalids Stockcodes
- 2 Negative values in Unit Price
## Data Cleaning Process
- Seperate Negative Values in Quantity
- Seperate Negative values in Price
- Removed rows where Stockcode is Invalid
- Renamed the Description to Products
- Filled missing values in CustomerID using forward fill
- Convert CustomerID datatype to Integer
- Convert the Invoicedate to Datetime Format
- Dropped the Duplicates values
# Exploratory Data Analysis(EDA)
## Key Insights
### Top 5 selling Products by Quantity 
- PAPER CRAFT , LITTLE BIRDIE	(80,995 units sold)
- MEDIUM CERAMIC TOP STORAGE JAR (78,033 units sold)
- JUMBO BAG RED RETROSPOT (48,371 units sold)
- WHITE HANGING HEART T-LIGHT HOLDER (37,872 units sold)
- ASSORTED COLOUR BIRD ORNAMENT (36,362 units sold)
### Top 5 selling products by Sales
-REGENCY CAKESTAND 3 TIER 174156.54
- PAPER CRAFT , LITTLE BIRDIE 168469.6
- WHITE HANGING HEART T-LIGHT HOLDER 106236.72
- PARTY BUNTING 99445.23
- JUMBO BAG RED RETROSPOT 94159.81
### Top 5 Countries by Sales
- United Kingdom 8187806.364
- Netherlands 284661.540
- EIRE 263276.820
- Germany	221698.210
- France 197403.900
# VISUALIZATION
![image](https://github.com/user-attachments/assets/e13b6713-b50a-4151-9c7a-1fdec75dc25c)

![image](https://github.com/user-attachments/assets/fc472172-6f9e-45ff-9874-fa6c2e260397)

![image](https://github.com/user-attachments/assets/0ed54128-038f-4d60-8744-2388c5e090b4)

![image](https://github.com/user-attachments/assets/c62fdb3d-9222-41db-92aa-302b838c8f2d)

![image](https://github.com/user-attachments/assets/0c61d6e9-0e94-404c-b11c-1c8d77381b05)

![image](https://github.com/user-attachments/assets/b93d1409-9847-48c9-a066-758093ba0847)

![image](https://github.com/user-attachments/assets/486051fb-d266-4760-9e78-45733ff80d64)

![image](https://github.com/user-attachments/assets/5d676ad8-66ad-462a-a9f4-cdbdfaac7d85)


# Data Preprocessing
- Dropped Irrelevant columns(InvoiceNo, StockCode, Product, InvoiceDate, CustomerID, Quantity, UnitPrice)
- Encoded Months and Days
# FEATURE ENGINEERING
## Total Sales
online_retail["TotalSales"]= online_retail["Quantity"] * online_retail["UnitPrice"]
- Extracted Year,Month,Week,Period of Days from InvoiceDate
# CLUSTERING CUSTOMER SEGMENTATION
- Calculated Recency as the number of days since last purchase
- Calculated Frequency as the number of purchase made
- Grouped Customers with their purchase behaviour (high,medium and low purchases)
# RECOMMENDATION
- Geographical : UK dominates in revenue ,

- 
  



