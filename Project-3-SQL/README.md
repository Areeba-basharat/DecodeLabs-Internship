# DecodeLabs Internship - Data Analytics

## Project 3: SQL Data Analysis

### Overview
This project is part of the DecodeLabs Data Analytics Internship. The goal 
was to use SQL to query the cleaned dataset (from Project 1) and pull out 
useful business insights -- things like top-selling products, revenue by 
payment method, average order values, and monthly trends.

The queries were run using SQLite (through Python) on the same 1,200-order 
dataset used in Project 1 and Project 2.

### Dataset Overview
- **Table:** orders
- **Total Records:** 1,200 orders
- **Columns:** 14
- **Date Range:** January 2023 - June 2025

### Project Requirements
According to the DecodeLabs Project 3 guidelines, the main requirements were:
- Write SELECT queries
- Use WHERE, ORDER BY, and GROUP BY
- Perform basic aggregations (COUNT, SUM, AVG)

### What I did

**1. Filtering with WHERE**
Wrote queries to filter orders by specific conditions, like payment method, 
year, and whether a coupon was used.

**2. Sorting with ORDER BY**
Found the 10 highest-value orders by sorting TotalPrice in descending order.

**3. Grouping and Counting**
Used GROUP BY with COUNT to find how many orders were placed for each 
product.

**4. Aggregations (SUM, AVG)**
Calculated total revenue by payment method (SUM) and average order value 
by referral source (AVG).

**5. Filtering Groups with HAVING**
Used HAVING to find which products have an average order value above 
Rs. 1,000.

**6. Combined Aggregations**
Wrote a query that gets order count, total revenue, and average order 
value together, grouped by order status.

**7. Date and Pattern Filtering**
Filtered orders placed in 2024, and separately looked at orders where no 
coupon was used.

**8. Monthly Trend**
Grouped orders by year-month to see how revenue changed over time.

### Key Findings
- Printer (181 orders) and Tablet (179 orders) are the most ordered products; 
  Phone (156 orders) is the least, though the numbers are all fairly close.
- Credit Card is the top revenue-generating payment method (Rs. 263,847.63), 
  followed closely by Online and Cash -- no single method dominates.
- Facebook has the highest average order value among referral sources 
  (Rs. 1,098.29), even though Instagram brings in more total orders.
- 5 out of 7 products have an average order value above Rs. 1,000, with 
  Laptop at the top (Rs. 1,110.56).
- Cancelled orders generated the highest total revenue by status 
  (Rs. 276,396.21) -- worth flagging since that's revenue that was almost 
  captured.
- Monthly revenue fluctuates a fair amount (e.g. Rs. 63,836.84 in May 2023 
  vs Rs. 27,751.71 in April 2023), so demand doesn't follow one obvious 
  seasonal pattern in this sample.

### Files
- `DecodeLabs_Project3_Queries.sql` — all 10 SQL queries used
- `DecodeLabs_Project3_SQL_Analysis.xlsx` — query results and key findings

### Tools Used
SQLite (via Python), Excel
