# Superstore Sales Dashboard

## Overview

This project presents an interactive sales dashboard developed in Microsoft Power BI using the Superstore dataset. The dashboard provides a comprehensive view of business performance by analysing revenue, profit, customer activity, product performance, shipping methods, and regional sales.

The objective of the report is to transform raw transactional data into meaningful insights that support business decision-making through interactive visualisations and key performance indicators (KPIs).

---


## Project Objectives

The dashboard was developed to:

- Monitor overall business performance.
- Analyse revenue and profit across different dimensions.
- Identify high-performing products and cities.
- Compare sales across regions and shipping modes.
- Understand customer purchasing patterns.
- Enable interactive exploration through report filters.

---

## Tools and Technologies

- Microsoft Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Data Modelling
- Data Visualisation

---

## Dataset

The project uses the Sample Superstore dataset containing approximately 10,000 sales records.

The dataset includes information on:

- Orders
- Customers
- Products
- Sales
- Revenue
- Profit
- Shipping Modes
- Regions
- States
- Cities
- Categories
- Sub-Categories

---

## Dashboard Metrics

The report tracks the following key business metrics:

| Metric | Description |
|---------|-------------|
| Total Revenue | Overall revenue generated |
| Total Orders | Total number of orders |
| Total Customers | Number of unique customers |
| Total Profit | Overall business profit |

---

## Dashboard Visualisations

The report contains the following visualisations:

- Revenue by City
- Revenue by Shipping Mode
- Top 10 Products by Revenue
- Revenue by Region
- Orders by Customer Segment
- Product Sub-Category Filter (Slicer)

Each visual interacts dynamically with the others, allowing users to drill into specific areas of interest.

---

## DAX Measures

The dashboard makes use of several custom DAX measures.

### Total Revenue

```DAX
Total Revenue =
SUM('Sample - Superstore'[Revenue])
```

### Total Profit

```DAX
Total Profit =
SUM('Sample - Superstore'[Profit])
```

### Total Orders

```DAX
Total Orders =
DISTINCTCOUNT('Sample - Superstore'[Order ID])
```

### Total Customers

```DAX
Total Customers =
DISTINCTCOUNT('Sample - Superstore'[Customer ID])
```

### Profit Margin

```DAX
Profit Margin =
DIVIDE(
    SUM('Sample - Superstore'[Profit]),
    SUM('Sample - Superstore'[Revenue]),
    0
)
```

---

## Key Insights

The dashboard reveals several business insights, including:

- Standard Class shipping generates the highest revenue.
- Revenue is concentrated among a relatively small number of cities.
- The Consumer segment contributes the largest share of total orders.
- Revenue distribution differs significantly across regions.
- A small group of products accounts for a substantial proportion of overall revenue.

---

## Skills Demonstrated

This project demonstrates proficiency in:

- Data Cleaning and Preparation
- Data Modelling
- DAX Measure Development
- Business Intelligence
- Dashboard Design
- Interactive Reporting
- KPI Development
- Data Storytelling
- Performance Analysis

---

## Future Enhancements

Potential improvements include:

- Time intelligence measures (YTD, MTD, YoY)
- Additional profitability analysis
- Customer retention metrics
- Drill-through report pages
- Custom tooltip pages
- Forecasting visualisations
- Navigation using bookmarks and buttons
- Executive summary page

---

## Author

**Jonathan Ogana**

Data Analyst specialising in SQL, Excel, Power BI, and Python.

---

## Acknowledgements

This project was developed as part of my practical data analytics training with **AnalystLab Africa**. The dashboard reflects concepts learned and applied throughout the programme using the Sample Superstore dataset.