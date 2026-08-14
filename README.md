# Sales Analysis

## Project Overview

This project analyzes transaction-level sales data to evaluate product profitability and monthly sales performance. SQL was used to transform raw sales data into meaningful business metrics and identify changes in product profitability over time.
## Key Metrics

* **Profit per Unit** — Difference between unit selling price and unit cost
* **Profit per Transaction** — Profit per unit multiplied by quantity sold
* **Profit Margin** — Profit as a percentage of selling price
* **Markup Percentage** — Profit as a percentage of unit cost
* **Monthly Profit** — Total transaction profit for each product and month
* **Month-over-Month Profit Change** — Change in monthly product profit compared with the previous month

## SQL Techniques Used

* Nested CTEs
* Aggregate functions
* DATE_TRUNC()
* Calculated fields - SUM() and AVG()
* Window functions
* LAG()
* PARTITION BY

## Analysis Process

The analysis is structured in two main stages.

### 1. Transaction-Level Analysis

The first CTE calculates profitability metrics for each sales transaction, including profit per unit, profit per transaction, markup percentage, and profit margin.

### 2. Monthly Product Analysis

The second stage aggregates the transaction-level data by product and month. Monthly profit, quantity sold, and profitability metrics are calculated before using the LAG() window function to compare each products performance with the previous month.

## Business Applications

This type of analysis could help a business:

* Identify highly profitable products
* Monitor changes in product performance
* Evaluate pricing and cost relationships
* Track profitability trends over time
