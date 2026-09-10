# DecodeLabs Data Analytics Internship – Project 2
## Exploratory Data Analysis (EDA)

### Project Overview

This project is part of the DecodeLabs Data Analytics Internship.

The purpose of this project is to perform Exploratory Data Analysis (EDA) on an order dataset and understand the patterns, trends, distributions, relationships, and outliers present in the data.

The analysis was performed using Excel and focuses on descriptive statistics, trend analysis, outlier detection, correlation analysis, and business-related observations.

---

## Dataset Overview

- **Total Records:** 1,200 orders
- **Number of Columns:** 14
- **Date Range:** January 2023 – June 2025
- **Main Numeric Columns:**
  - Quantity
  - UnitPrice
  - ItemsInCart
  - TotalPrice

---

## Project Requirements

According to the DecodeLabs Project 2 guidelines, the main requirements are:

- Calculate basic statistics such as **mean, median, and count**
- Identify **trends and outliers**
- Summarize **key observations**

Additional analysis was performed to make the EDA more useful and understandable.

---

## Analysis Performed

### 1. Descriptive Statistics

Basic statistical measures were calculated for the main numeric columns, including:

- Count
- Mean
- Median
- Mode
- Standard Deviation
- Minimum
- Maximum

### 2. Five-Number Summary

The following values were calculated for the numeric variables:

- Minimum
- Q1 (25th percentile)
- Median
- Q3 (75th percentile)
- Maximum

The IQR (Interquartile Range) was also calculated.

---

### 3. Outlier Detection

The **IQR method** was used to identify potential outliers.

Formula used:

**IQR = Q3 − Q1**

**Lower Bound = Q1 − 1.5 × IQR**

**Upper Bound = Q3 + 1.5 × IQR**

The analysis found:

- **8 potential TotalPrice outliers**
- These represent approximately **0.67% of the dataset**
- The upper IQR limit for TotalPrice is approximately **Rs. 3,330.41**

The outliers were not automatically removed because a statistical outlier is not necessarily a data error. The high-value orders should be reviewed in their business context.

---

### 4. Trend Analysis

Monthly and yearly trends were analyzed using:

- Number of orders
- Total revenue

The analysis showed that **June** was the strongest month in the dataset.

- **Orders:** 147
- **Revenue:** approximately Rs. 170,616

Yearly results were also compared to understand changes in order volume and revenue.

---

### 5. Correlation Analysis

Correlation analysis was performed to understand relationships between numerical variables.

Important results include:

- **UnitPrice vs TotalPrice:** 0.72
- **Quantity vs TotalPrice:** 0.62
- **Quantity vs ItemsInCart:** 0.65
- **ItemsInCart vs TotalPrice:** 0.39
- **UnitPrice vs ItemsInCart:** 0.00

UnitPrice had the strongest relationship with TotalPrice among the analyzed variables.

---

### 6. Data Visualization

The following visualizations were included:

- TotalPrice distribution histogram
- TotalPrice boxplot
- Trend analysis
- Statistical summaries

The histogram helps show the distribution of TotalPrice, while the boxplot provides visual evidence of the potential outliers.

---

## Key Findings

1. The dataset contains **1,200 orders** covering January 2023 to June 2025.

2. The average TotalPrice is **Rs. 1,053.97**, while the median is **Rs. 823.62**. The difference indicates that TotalPrice is right-skewed, with some high-value orders increasing the average.

3. The IQR method identified **8 potential high-value outliers** in TotalPrice.

4. **June** had the highest number of orders and the highest revenue in the analyzed monthly data.

5. UnitPrice has a strong positive relationship with TotalPrice, with a correlation of **0.72**.

6. Quantity also has a positive relationship with TotalPrice, with a correlation of **0.62**.

7. Products, payment methods, and referral sources are relatively balanced in the dataset, without one category completely dominating the results.

---

## Business Recommendations

Based on the analysis:

- Track both **mean and median order value** to understand typical customer spending.
- Review the **8 high-value orders** to determine whether they are genuine bulk purchases or possible data issues.
- Consider preparing inventory and resources before **June**, since it is the strongest month in this dataset.
- Monitor product pricing because UnitPrice has a strong relationship with TotalPrice.
- Continue monitoring different payment and referral channels rather than depending on only one channel.

---

## Data Quality Note

The supplied dataset contains **309 missing CouponCode values**.

These values were documented in the analysis rather than replaced with invented coupon codes because CouponCode is not required for the main numerical EDA calculations.

The missing-value information can be found in the **Data_Quality** sheet.

---

## Workbook Contents

The final Excel workbook contains the following sheets:

- **Summary_Statistics** – Descriptive statistics
- **Five_Number_Summary** – Five-number summary and IQR
- **Outliers** – Outlier calculations and flagged orders
- **Trends** – Monthly and yearly trends
- **Correlation** – Correlation analysis
- **Charts** – Data visualizations
- **Key_Findings** – Main observations
- **Recommendations** – Business recommendations
- **Methodology** – Analysis methods used
- **Data_Quality** – Missing-value information

---

## Conclusion

This project demonstrates the use of Exploratory Data Analysis to understand a dataset through descriptive statistics, trends, distributions, outlier detection, correlation analysis, visualization, and business insights.

The analysis helped identify important patterns in order values, monthly performance, relationships between numerical variables, and unusually high-value orders.

---

### Tools Used

- Microsoft Excel
- Exploratory Data Analysis
- Descriptive Statistics
- IQR Outlier Detection
- Correlation Analysis
- Data Visualization

---

**Project:** DecodeLabs Data Analytics Internship – Project 2  
**Topic:** Exploratory Data Analysis (EDA)
