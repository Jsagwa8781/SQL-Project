# SQL-Project

# ACDOCA and CostCenter SQL Script

This script creates two tables, `ACDOCA` and `CostCenter`, populates them with sample data, performs operations, and generates queries for data visualization in Power BI.

## ACDOCA Table

The `ACDOCA` table stores transaction data with the following columns:

- `Ledger`: Ledger identifier
- `CompanyCode`: Company code identifier
- `FiscalYear`: Fiscal year of the transaction
- `DocumentNumber`: Document number of the transaction
- `PostingItem`: Posting item identifier
- `ReferenceNumber`: Reference number of the transaction
- `TransactionCurrency`: Currency of the transaction

## CostCenter Table

The `CostCenter` table stores financial data related to company codes with the following columns:

- `CompanyCode`: Company code identifier
- `SumAmountTransactionCurrency`: Total transaction amount in transaction currency
- `SumAmountCompanyCodeCurrency`: Total transaction amount in company code currency
- `SumAmountGlobalCurrency`: Total transaction amount in global currency

## Operations

- Rows are deleted from the `CostCenter` table to create an equal number of rows in both tables.

## Data Analysis Queries 

The following SQL queries provide insights to analyze the financial data stored in the ACDOCA and CostCenter tables:

1. **Joining Tables** A query that joins the ACDOCA and CostCenter tables, fetching data related to company codes, transaction amounts, and transaction details.

2. **Transaction Amounts by Fiscal Year and Currency (2022 and 2023)** Two queries that filter and display transaction amounts based on fiscal year and specific currencies.

3. **Transaction Amount Distribution by Company Code and Currency** A query that calculates the total transaction amount for each company code and currency combination, providing insights into transaction trends.

4. **Company Code Transaction Amount Share Over Fiscal Years (2022 and 2023)** Two queries that analyze the share of transaction amounts for each company code in specific fiscal years.

5. **Transaction Amount Trend Over Fiscal Years by Ledger** A query that displays the trend of transaction amounts over fiscal years, grouped by the ledger attribute.

6. **Transaction Amount Ratio by Ledger and Fiscal Year** A query that calculates the ratio of transaction amounts for different ledgers in each fiscal year.

## Usage

1. Run the provided SQL script in your Microsoft SQL Server database environment.
2. Use the generated tables and data to connect with Power BI and create visualizations and dashboards.

Note: This script includes sample data and queries for illustrative purposes. Modify and adapt it to your actual data and requirements.

