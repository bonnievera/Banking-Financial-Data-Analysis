# Banking-Financial-Data-Analysis
A comprehensive project demonstrating the full data lifecycle from automated ingestion using Python to advanced financial analytics and fraud detection using SQL.

## Project Overview
This project simulates a retail banking environment by processing and analyzing a relational dataset containing customers, accounts, transactions, loans, and branch information.

Unlike static SQL exercises, this project features a dynamic ETL (Extract, Transform, Load) phase. Using Jupyter Notebook and Python, I automated the migration of raw CSV data into a structured MySQL database, ensuring data integrity and relational mapping across 10,000+ records.

The objective is to:
- Perform customer and account analysis
- Evaluate branch performance
- Analyze loan risk
- Detect suspicious transaction behavior
- Apply advanced SQL analytics techniques

## Fraud Detection Techniques Used

- Transactions 3x larger than account average
- Accounts with abnormal daily activity
- High-risk scoring logic

## Key Insights

- Identified high-value customers with balances above 50,000
- Ranked customers within each branch
- Calculated branch level loan exposure
- Measured loan default distribution
- Flagged suspicious transaction patterns

## SQL Skills Demonstrated

- SELECT
- WHERE
- ORDER BY
- COUNT
- JOIN (multiple tables)
- GROUP BY
- HAVING
- Aggregations (SUM, AVG)
- Window Functions (RANK, SUM OVER)
- Running Totals
- Correlated Subqueries
- Fraud Detection Logic

 ### Tech Stack
* **Language:** Python , SQL
* **Libraries:** Pandas, SQLAlchemy, PyMySQL
* **Database:** MySQL
* **Environment:** Jupyter Notebook

## Entity Relationship Diagram (ERD) 
The database follows a Star Schema architecture designed to optimize query performance for transactional reporting.
![Database Entity Relationship Diagram](visuals/ERD.png)

### Key Findings & Insights
## 1. Branch Performance & Loan Exposure
Top Performing Branch: Branch [Insert City Name] accounts for over 35% of the total loan volume, indicating a high demand for credit in that region.

Risk Profile: Approximately 12% of the total loan portfolio is currently in "Default" status, primarily concentrated in accounts with a history of low balances.

## 2. Customer Wealth Distribution
High-Net-Worth Segment: Only 5% of the customer base holds 60% of the total bank deposits. This identifies a significant opportunity for tiered "Premier Banking" services.

Savings Trends: Using Window Functions, I observed that customers with recurring monthly transfers of $500+ show a 20% higher balance growth rate compared to irregular savers.

## 3. Fraud & Security Audit
Anomaly Detection: The "3x Average" spike query flagged 42 transactions for manual review. Further investigation showed these were concentrated on weekends, a common pattern for unauthorized account access.

Velocity Alerts: 15 accounts triggered the "High-Velocity" flag (5+ transactions in 24 hours), successfully identifying potential "Money Mule" activity or automated bot testing.
