# Customer Segmentation using RFM Model

## The purpose of this project is to share some experiences I had with customer segmentation using a RFM model. Also I learned a lot from the course "Customer Segmentation in Python" in DataCamp. I tried to apply what I learned into this project as well.

## RFM is one of the most widely used techniques for selecting significant customers. It is a very popular customer segmentation technique that uses the customers’ past purchase behavior to divide them into different groups based on similarities. The name RFM stands for Recency, Frequency, and Monetary value.

* Recency - days since last customer transaction
* Frequency - number of transactions in the last 12 months
* Monetary Value - total spend in the last 12 months
## Context:
Typically e-commerce datasets are proprietary and consequently hard to find among publicly available data. However, The UCI Machine Learning Repository has made this dataset containing actual transactions from 2010 and 2011. The dataset is maintained on their site, where it can be found by the title "Online Retail".

## Data: https://www.kaggle.com/carrie1/ecommerce-data
### This is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers."
### This dataframe contains 8 variables that correspond to:
1. InvoiceNo: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation.
2. StockCode: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
3. Description: Product (item) name. Nominal.
4. Quantity: The quantities of each product (item) per transaction. Numeric.
5. InvoiceDate: Invice Date and time. Numeric, the day and time when each transaction was generated.
6. UnitPrice: Unit price. Numeric, Product price per unit in sterling.
7. CustomerID: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
8. Country: Country name. Nominal, the name of the country where each customer resides.
#### For easy analysis, I defined the data scope:
* Country: United Kingdom
* Timeframe: 1 year (from 2010-12-10 to 2011-12-09)
* CustomerID is not null
* Do not consider returning
