\# Power BI E-Commerce Sales Analysis



!\[Power BI](https://img.shields.io/badge/Power%20BI-Data%20Analysis-F2C811?style=for-the-badge\&logo=powerbi\&logoColor=black)

!\[Data Transformation](https://img.shields.io/badge/Data-Transformation-blue?style=for-the-badge)

!\[Data Modeling](https://img.shields.io/badge/Data-Modeling-2E75B6?style=for-the-badge)



\## Project Overview



This project is an E-Commerce Sales Analysis developed using Microsoft Power BI as part of an assignment on \*\*Data Transformation \& Data Modeling\*\*.



The project demonstrates an end-to-end Business Intelligence workflow, beginning with importing raw sales data and continuing through data transformation, data cleaning, data merging, grouping and aggregation, data modeling, visualization, and business-oriented interpretation.



The final Power BI report contains:



\- A Sales Performance Dashboard

\- An Insights \& Recommendations page

\- Interactive filtering

\- Transformed and summarized data

\- Relationships between relevant tables

\- Business-focused analysis of sales, profitability, orders, and target performance



\---



\## Business Objective



The objective of this analysis is to transform transactional e-commerce data into meaningful business information that can support the evaluation of:



\- Sales performance

\- Category-level performance

\- Profitability

\- Order profitability status

\- Monthly sales trends

\- Actual sales versus target performance

\- Areas requiring business attention



The analysis also demonstrates how Power BI can be used to convert raw operational data into an interactive analytical report.



\---



\## Assignment Objectives



The project addresses the following major requirements:



1\. Import the provided sales datasets into Power BI.

2\. Transform and clean the data using Power Query.

3\. Restrict the `List of Orders` table to the first 500 rows.

4\. Set appropriate data types for date and numerical fields.

5\. Format customer names consistently using proper case.

6\. Create a combined `Location` field from City and State.

7\. Calculate `Profit Margin`.

8\. Create a `Profit Status` classification.

9\. Merge `List of Orders` and `Order Details` using `Order ID`.

10\. Identify missing values and determine an appropriate handling strategy.

11\. Check duplicate records and determine an appropriate handling strategy.

12\. Apply sorting and filtering operations.

13\. Create summary queries for grouping and aggregation.

14\. Establish relationships between the required tables.

15\. Build an interactive Power BI dashboard.

16\. Present data-driven insights and recommendations.



\---



\## Dataset Overview



The assignment provided three CSV datasets:



\- `List of Orders.csv`

\- `Order Details.csv`

\- `Sales target.csv`



The datasets contain information related to orders, customers, locations, products/categories, sales amounts, profit, and sales targets.



For the assignment analysis, the `List of Orders` data was restricted to the first \*\*500 records\*\*, as specified in the requirements.



\---



\## Tools \& Technologies



| Tool | Purpose |

|---|---|

| Microsoft Power BI Desktop | Data modeling, visualization and dashboard development |

| Power Query | Data transformation and preparation |

| CSV | Source data format |

| GitHub | Project documentation and portfolio presentation |



\---



\# Data Transformation



Data preparation was performed using Power Query.



\### Key transformations



\### 1. Row Restriction



The `List of Orders` table was restricted to the first \*\*500 rows\*\*, as required by the assignment.



\### 2. Data Type Standardization



Appropriate data types were applied to important fields, including:



\- `Order Date` → Date

\- `Amount` → Fixed Decimal Number

\- `Target` → Fixed Decimal Number



\### 3. Customer Name Formatting



The `CustomerName` column was formatted using proper case to improve consistency and readability.



\### 4. Location Creation



The `State` and `City` fields were combined into a new:



`Location`



field using the required:



`City, State`



format.



\### 5. Profit Margin



A custom column named:



`Profit Margin`



was created using:



`Profit / Amount`



This provides a relative measure of profitability.



\### 6. Profit Status



A conditional column named:



`Profit Status`



was created according to the assignment requirements:



| Profit condition | Profit Status |

|---|---|

| Profit < 0 | Loss |

| Profit = 0 | Break-Even |

| Profit > 0 | Profit |



\---



\# Data Merging



The `List of Orders` and `Order Details` tables were merged using:



`Order ID`



The resulting combined dataset was named:



`Orders Data`



This created a consolidated table containing order-level and order-detail information for analysis.



\---



\# Missing \& Duplicate Data Handling



Missing values were reviewed during the data preparation process and an appropriate handling strategy was considered based on the nature and context of the fields.



Duplicate records were also checked and a suitable strategy was determined to prevent inappropriate duplication from affecting the analysis.



The purpose of these checks was to improve data quality while avoiding unnecessary alteration of valid transactional records.



\---



\# Sorting \& Filtering



The transformed `Orders Data` table was used for sorting and filtering analysis.



The assignment required:



\- Sorting `Order Date` in descending order to examine recent orders.

\- Filtering the data by a specific state, such as Tamil Nadu, for regional analysis.



These operations demonstrate how transactional data can be explored according to specific business criteria.



\---



\# Grouping \& Aggregation



Additional queries were created to support grouped analysis.



The project contains summary queries for:



\### Order Details Summary



Used to summarize order-level information, including order counts.



\### Order Details Category Summary



Used to calculate category-level summary information, including average profit by category.



\### Sales Target Summary



Used to aggregate sales target information by month.



These summarized datasets support both the analytical workflow and dashboard development.



\---



\# Data Modeling



Relationships were established between the relevant tables using common business keys.



The primary modeling relationships include:



\- `Order Details` ↔ `List of Orders` using `Order ID`

\- `Order Details` ↔ `Sales target` using `Category`



The project also contains the transformed and summarized tables required for the assignment analysis.



The model was reviewed using Power BI's Model view and relationship management functionality.



\---



\# Power BI Dashboard



The final report contains an interactive \*\*Sales Performance Dashboard\*\*.



!\[Sales Performance Dashboard](Screenshots/Sales\_Performance\_Dashboard.png)



\### Dashboard Components



The dashboard includes:



\#### KPI Cards



\- Total Sales

\- Total Profit

\- Total Orders



\#### Sales Analysis



\- Sales by Category



\#### Profitability Analysis



\- Profit by Category

\- Orders by Profit Status



\#### Performance Analysis



\- Actual Sales vs Target

\- Monthly Sales Trend



\#### Interactive Filters



\- Category

\- Profit Status



These components provide a consolidated view of sales performance and profitability.



\---



\# Key Data-Driven Insights



The dashboard analysis produced the following key findings.



\### 01 | Overall profitability is negative



Total sales are approximately \*\*₹6.09K\*\*, while total profit is approximately \*\*-₹2.22K\*\*, indicating an overall loss position within the analyzed dataset.



\### 02 | Furniture has the highest sales but the largest profit concern



Furniture generates approximately \*\*₹3.0K\*\* in sales, making it the strongest sales category shown.



However, it records approximately \*\*-₹2.5K\*\* in profit, making it the largest category-level profitability concern.



\### 03 | Electronics is the only profitable category shown



Electronics generates approximately \*\*₹0.4K\*\* in profit.



By comparison:



\- Clothing records approximately \*\*-₹0.1K\*\*

\- Furniture records approximately \*\*-₹2.5K\*\*



\### 04 | Order profitability is mixed



Approximately:



\- \*\*46.15%\*\* of orders are classified as Profit

\- \*\*30.77%\*\* are classified as Loss

\- \*\*23.08%\*\* are classified as Break-Even



This indicates that positive-profit orders represent the largest group, but a substantial proportion of orders are either loss-making or break-even.



\---



\# Business Recommendations



The findings suggest several areas that could be investigated from a business perspective.



\### 01 | Review Furniture profitability



Investigate:



\- Product-level costs

\- Pricing

\- Discounts

\- Profit margins

\- Low-performing products



Furniture generates the highest sales but also the largest loss, making profitability improvement in this category a priority.



\### 02 | Protect and expand profitable Electronics sales



Identify the products, pricing conditions and sales characteristics contributing to Electronics' positive profitability.



The objective should be to understand what is working and determine whether those conditions can be maintained or expanded.



\### 03 | Reduce loss-making orders



Analyze orders classified as Loss to identify recurring causes.



Potential areas for investigation include:



\- Pricing

\- Discounts

\- Product selection

\- Cost structure

\- Category-level profitability



\### 04 | Monitor target performance



Actual sales should be compared with monthly targets consistently.



Periods showing significant differences between actual sales and target performance should be investigated to understand the underlying business factors.



\---



\# E-Commerce Industry Perspective



The findings also illustrate several broader considerations relevant to e-commerce businesses.



\## Revenue does not necessarily equal profitability



A category can generate high sales while still producing poor or negative profitability.



Therefore, e-commerce performance should be evaluated using both:



\- Revenue

\- Profitability



rather than sales volume alone.



\## Category-level profitability monitoring



Category-level analysis can help businesses identify products or categories where strong sales are accompanied by unfavorable margins.



This can support decisions related to:



\- Product portfolio management

\- Pricing

\- Promotions

\- Discounts

\- Cost control



\## Profitability-based decision making



Order-level profitability classification can help organizations distinguish between:



\- Profitable transactions

\- Loss-making transactions

\- Break-even transactions



This can provide a foundation for investigating recurring patterns in commercial performance.



\## Sales target monitoring



Comparing actual sales with targets on a monthly basis can help management identify periods of underperformance or stronger-than-expected performance.



\## Data-driven commercial strategy



Interactive BI dashboards can provide decision-makers with a consolidated view of sales, profitability, order performance and targets, helping transform transactional data into actionable business information.



> \*\*Note:\*\* These industry perspectives are broader business interpretations of the project findings. They should not be interpreted as conclusions about the entire e-commerce industry based solely on this assignment dataset.



\---



\# Key Business Questions Answered



The dashboard was designed to help answer questions such as:



1\. How much total sales were generated?

2\. Is the business operating at a profit or loss?

3\. How many orders were analyzed?

4\. Which category generates the highest sales?

5\. Which category generates the highest profit or loss?

6\. What proportion of orders are profitable, loss-making or break-even?

7\. How are actual sales performing against targets?

8\. How do sales change over time?

9\. Which areas require further business investigation?



\---



\# Limitations



The analysis should be interpreted within the scope of the assignment dataset.



Key limitations include:



\- The `List of Orders` data was restricted to the first 500 rows as required by the assignment.

\- The analysis is based only on the fields available in the provided datasets.

\- The findings should not automatically be generalized to an entire e-commerce organization or industry.

\- Further analysis using product-level costs, customer acquisition costs, logistics costs, discount information and other commercial variables could provide deeper profitability insights.



\---



\# Conclusion



This project demonstrates an end-to-end Power BI workflow covering:



\*\*Data Import → Data Transformation → Data Cleaning → Data Merging → Data Aggregation → Data Modeling → Data Visualization → Business Insights\*\*



The resulting dashboard transforms transactional e-commerce data into an interactive analytical report covering sales, profitability, order status and target performance.



The analysis highlights an important business finding: \*\*strong sales performance does not necessarily translate into strong profitability\*\*.



In particular, Furniture generates the highest sales but also the largest category-level loss, while Electronics is the only profitable category shown in the analysis.



The project therefore demonstrates not only technical Power BI capabilities, but also the importance of connecting data analysis with business interpretation and decision-making.



\---



\# Project Structure



```text

PowerBI-Ecommerce-Sales-Analysis/

│

├── README.md

│

├── PowerBI/

│   └── Power BI Assignment 1 - Data Transformation \& Data Modeling.pbix

│

├── Screenshots/

│   ├── Sales\_Performance\_Dashboard.png

│   └── Insights\_Recommendations.png

│

└── Documentation/



\---



\# Insights \& Recommendations



The project includes a dedicated Insights \& Recommendations page summarizing the principal findings and recommended business actions.



!\[Insights \& Recommendations](Screenshots/Insights\_Recommendations.png)



\---



\## Author



\*\*Gloriya V. Johnson\*\*



Data Analytics Trainee | Power BI | Excel | SQL | Python



\---



\## Project Type



\*\*Academic / Portfolio Data Analytics Project\*\*



\*\*Domain:\*\* E-Commerce Sales Analytics  

\*\*Platform:\*\* Microsoft Power BI  

\*\*Focus:\*\* Data Transformation, Data Modeling, Business Intelligence \& Data-Driven Decision Making

