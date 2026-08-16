# Finance & Performance Analysis Dashboard

A Power BI dashboard tracking company expenses, income versus expenses, and spending patterns across accounts, companies, and time.

## Business Question

Where is company spending concentrated, how does income compare to expenses over time, and which accounts, categories, and time periods drive the biggest swings?

## Method

- Imported and cleaned transaction-level data in Power Query
- Built DAX measures (Total Income, Total Expenses, Net Cashflow) and calculated columns (Weekday, Month-Year)
- Built visuals covering spending by category, subcategory, weekday, month, account, and company
- Added slicers for Company, Account, and Date to make the dashboard interactive

## Headline Findings

- Income exceeded expenses in every month, for a total net cash flow of $64.4K in 2023
- Spending is evenly spread across categories, accounts, and companies rather than concentrated in a few outliers
- Weekends see the highest spending of the week

## Questions the Dashboard Answers

- Which expense categories and subcategories contribute the most to total spending
- Which days of the week see the most and least spending
- How monthly income and expenses compare over time
- The overall difference between total income and total expenses
- Which account types account for the most debit transactions
- How debit transactions are distributed across companies

## Files

- `finance-expense-dashboard.pbix`: full Power BI file
- `dashboard-notes.pdf`: project write-up

## Sources and Reference

Dataset: [Finance_Expenses.csv, Anish7000/Finance-Analysis-Dashboard](https://github.com/Anish7000/Finance-Analysis-Dashboard). This project was built independently from the KPI questions and raw dataset published in that repository, then compared against its dashboard.
