# Northwind Business Analysis Project

## OVERVIEW

This project is a hands-on SQL data analysis case study built around the Northwind database,a standard retail datset. It demosrates how to query, extract ,analyse and present business insights from a relational database using SQL. This project covers real-world data analysis tasks , from querying and exploring data to uncovering meaningful business insights.

## OBJECTIVES

The project aims to :
* Import and profile the Northwind dataset
* Understand the relationships between tables in the Northwind datasbase
* Write SQL queries to answer key business questions
* Draw insights that can support business decision-making
* Build a well documented, reproducible SQL project using Excel visualisations

## EXECUTIVE SUMMARY

This analysis of the Northwind dataset provides insight into customer activity, product performance, and overall business operations.

The company recorded a total of 830 orders, generating 126,579.04 in revenue, which reflects steady business performance. However, sales and activity are not evenly distributed, as a small number of customers contribute a large share of total orders.

A group of loyal customers plays a major role in revenue generation, making customer retention an important focus. In addition, shipping costs are concentrated among a few customers, indicating uneven logistics expenses across the customer base.

From a geographical perspective, although customers are spread across different countries, the majority of activity is concentrated in Brazil, France, and Germany. Among these, Brazil shows strong potential for further growth, making it a key market for expansion.

Product analysis shows that some categories dominate sales while others are less represented, suggesting an opportunity to improve product balance and explore underperforming categories.

Operational issues were also identified. Missing region data in several records points to data quality challenges, which may affect decision-making and planning. Additionally, 21 orders remain unshipped, highlighting possible delays in the fulfillment process.

The company works with a wide range of suppliers, which reduces dependence on a single source but may also create inefficiencies in cost management.

Overall, the business is performing well but can improve by focusing on data accuracy, operational efficiency, customer retention, and strategic expansion into high-performing regions.


## DATASET

The datset used is the Northwind SQLite database which was downloaded from kaggle. It contains retail business data across multiple tables, including:

* Customers
* Orders
* OrderDetails
* Products
* Suppliers
* CategoriesThe dataset used is the Northwind database.

[Northwind SQLite database](https://github.com/jpwhite3/northwind-SQLite3)


## TOOLS & TECHNOLOGIES

* SQL (SQLite Online)
* Excel (for analysis and visualisations)


## PROJECT WORKFLOW

### DATABASE ACCESSING

* Downloaded the Northwind [.sqlite](https://www.kaggle.com/datasets/munawarsaudagar/northwind-2000-sqlite) database from Kaggle

### DATA LOADING
  
* Imported the Northwind [.sqlite](https://www.kaggle.com/datasets/munawarsaudagar/northwind-2000-sqlite) database into SQLite Online

* Profiled tables and relationships

### SQL ANALYSIS AND QUERYING

* Wrote and executed queries to answer business-focused questions

* Applied concepts such as:

   - DISTINCT
   - NULL handling
   - Aggregate functions (SUM, COUNT, AVG)
   - GROUP BY
   - HAVING
   - Aliasing
 
### DATA EXPORTING

* Exported query results into Microsoft Excel files

### VISUALISATIONS

* Created visuals (bar, column, line) using Excel.
  
* Added titles and structured sheets for clarity.


## KEY BUSINESS QUESTIONS SOLVED

1. List of unique countries where customers are located [Q1](#q1-global-distribution-of-customer-base)
2. All customers who do not have a region assigned [Q2](#q2-incomplete-customer-data)
3. Total number of orders placed [Q3](#q3-order-volume-overview)
4. Total revenue using the Order Details table [Q4](#q4-total-revenue-generated)
5. Total number of products in each category [Q5](#q5-product-performance)
6. Customers who have placed more than 10 orders [Q6](#q6-high-value-customers)
7. Average freight cost per customer [Q7](#q7-average-order-value)
8. Suppliers who supply more than 5 products [Q8](#q8-suppliers-with-multiple-products)
9. Countries that have more than 5 customers [Q9](#q9-countries-with-high-customer-base)
10. Total number of orders that have not been shipped yet [Q10](#q10-delayed-or-unshipped-orders)


## SKILLS DEMOSTRATED

* SQL querying and database interaction
* Data cleaning and validation
* Business-oriented data analysis
* Data aggregation and summarisation
* Insight generation and reporting
* Data visualisation and storytelling
  

## KEY INSIGHTS

### Customer Geographic Reach
   Northwind's customers are spread across 21 countries worldwide, with Europe making up the bulk of the customer base, a sign of market depth that also points to untapped potential in other regions.

   - SQL QUERY

```sql
SELECT DISTINCT Country AS customer_country
FROM Customers c;
```
  



