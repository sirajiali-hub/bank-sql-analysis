# Bank Customer & Credit Risk Analysis SQL Project

SQL-driven analysis of a mid-sized bank's customer base, loan portfolio, 
transaction patterns, and marketing effectiveness.

## What This Project Does

Answers critical business questions a credit risk team and bank management 
would ask, using SQL queries on a relational database with 5 connected tables.

## Business Questions Answered

1. **Customer Segmentation** — Which demographics hold the most value?
2. **Credit Risk** — Which segments default most? Are bigger loans riskier?
3. **Revenue Analysis** — Where does transaction volume concentrate?
4. **Loan Portfolio Health** — How much capital is at risk from defaults?
5. **Marketing Effectiveness** — Which campaigns convert best?
6. **Risk Dashboard** — Full segment view combining all metrics

## SQL Skills Demonstrated

- Multi-table JOINs (2, 3, and 4 table joins)
- Aggregation (COUNT, SUM, AVG, ROUND)
- CASE WHEN conditional logic
- Subqueries and correlated subqueries
- Window functions (RANK, PARTITION BY)
- HAVING for group filtering
- NULLIF for safe division

## Database Schema

| Table | Rows | Key Columns |
|-------|------|-------------|
| customers | 11,162 | customer_id, age, job, education |
| accounts | 11,162 | account_id, balance, account_type |
| loans | 5,906 | loan_amount, interest_rate, loan_status |
| transactions | 61,276 | amount, transaction_type, transaction_date |
| campaign | 11,162 | contact_method, call_duration, subscribed_deposit |

## Key Findings

- Students have highest default rate (15.4%) despite smallest loans
- Services and blue-collar segments are overleveraged (loan-to-balance >1,300x)
- Savings accounts show negative net flow — withdrawal exceeds deposits
- Estimated default losses at 60% LGD quantified for IFRS 9 provisioning

## Tech Stack

Python, SQLite, pandas

## Author

Siraji Ali
