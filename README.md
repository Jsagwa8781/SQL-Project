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

## Data Visualization Queries

The following SQL queries provide insights for data visualization in Power BI:

1. **Transaction Currency Count by Fiscal Year**: Counts and sums transaction amounts by fiscal year and transaction currency.

2. **Top Companies by Total Global Amount**: Lists the top 10 companies by their total global amounts.

3. **Transaction Amount Trend Over Fiscal Years**: Displays transaction amount trends over fiscal years and company codes.

4. **Transaction Amount Distribution by Ledger and Fiscal Year**: Shows the distribution of transaction amounts by ledger and fiscal year.

5. **Transaction Amount Ratio by Transaction Currency**: Presents the transaction amount ratio by transaction currency.

6. **Sum Amounts by Transaction Currency and Posting Item**: Summarizes transaction amounts by fiscal year, company code, and posting item.

## Usage

1. Run the provided SQL script in your Microsoft SQL Server database environment.
2. Use the generated tables and data to connect with Power BI and create visualizations and dashboards.

Note: This script includes sample data and queries for illustrative purposes. Modify and adapt it to your actual data and requirements.

