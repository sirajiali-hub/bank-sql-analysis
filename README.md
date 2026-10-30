# Bank Customer and Credit Risk Analysis with SQL

**In one line:** Using SQL to answer the questions a bank manager asks about customers, loan defaults and marketing.

## The questions
1. Which customer groups default most on their loans?
2. How healthy is the loan book, and how much money is at risk?
3. Which customers respond best to marketing calls?

## What I did
1. Loaded five linked tables into a SQL database: customers, accounts, loans, transactions and marketing campaigns.
2. Joined the tables to link each customer to their account, loans and activity.
3. Grouped customers by job, education and loan size, and worked out default rates for each group.
4. Ranked customers by how much money they moved, and sized up the loan book by status.

## What I found
* **Defaults:** 9.9% of loans (586 of 5,906) have defaulted, about 9.1% of the loan book by value. At a 60% loss rate, that means expected losses of about 411 million.
* **Riskiest group:** students default most (15.4%), but there are only 52 student borrowers. Self employed borrowers default least (7.1%).
* **Loan size:** bigger loans are not riskier. Default rates stay between 8% and 11% at every loan size.
* **Savings accounts:** more money was withdrawn than deposited (about 12.5 million net outflow), worth watching.
* **Marketing:** students and retired customers sign up most (71% to 79% when called on a mobile phone), and mobile calls beat landline calls.

## Why it matters
Banks keep their data in databases. This shows I can pull clear business answers straight from them with SQL.

## Limitations
* Practice data based on a public bank marketing dataset, not a real bank's records.
* Some groups are small, so their rates can swing a lot.
* No dates are used, so it cannot show trends over time.

## How to run
1. Run `pip install pandas`
2. Open the notebook and run all cells. The SQL runs inside Python with SQLite.

**Tools:** SQL (SQLite), Python
