# Supermarket Sales Analysis — Power BI Dashboard

[![Power BI](https://img.shields.io/badge/Technology-Power%20BI-blue?logo=microsoft-power-bi&logoColor=white)](#) [![Author](https://img.shields.io/badge/Author-Katkam%20Sai%20Krishna-green)](#)

## Overview

This repository contains a multi-page Power BI dashboard and supporting assets for analyzing supermarket sales. The dashboard provides insights into sales performance, product trends, sales representative contributions, and financial/payment collection metrics to help stakeholders make data-driven decisions.

## Business Problem

Retail organizations accumulate large volumes of transactional data that are difficult to interpret without structured reporting. Decision-makers need consolidated dashboards that surface revenue trends, profitability, product performance, and collections status to monitor business health and prioritize actions.

This project converts raw sales transactions into actionable business insights via ETL, modeling, visualizations and KPI tracking.

---

## Key Features

- Executive Summary with high-level KPIs and trends
- Representative performance analysis (sales, AOV, contribution)
- Product performance and category analysis
- Financial & payment collection monitoring (paid vs due, outstanding dues)
- Interactive slicers and drill-downs (date range, region, representative, category)
- Reusable data model built with Power Query and DAX measures

---

## Dashboard Pages & Highlights

### Executive Summary
- Total Sales, Total Orders, Gross Profit
- Monthly Sales Trend, Sales by Category
- Top Products and Top Representatives

### Representative Performance
- Sales by Representative, Average Order Value (AOV)
- Customer tier distribution, Quantity sold, Profit contribution

### Product Performance
- Top-selling products, Category-level insights
- Product matrix and gross profit analysis

### Financial & Payment Analysis
- Payment status, Collection rate, Outstanding dues
- Payment trends and order status distribution

---

## Tech Stack

- Power BI (report & visualizations)
- Power Query (ETL)
- DAX (measures & KPIs)
- Excel, SQL (data prep & validation)

---

## Skills Demonstrated

- Data cleaning and transformation
- Data modeling and relationships in Power BI
- DAX for KPI and measure creation
- Dashboard and KPI design for business users
- Interactive reporting with filters and drill-downs

---

## Folder Structure

- dataset/ — source dataset(s) used for analysis
- dashboard/ — exported resources or documentation for the report
- images/ — screenshots used in this README
- Super Market Sales.pbix — Power BI report file
- README.md — project documentation

---

## Screenshots

<p align="center">
  <img width="900" alt="Executive Dashboard" src="https://github.com/user-attachments/assets/15d51855-8bd8-4987-a344-c76398cbb292" />
</p>

<p align="center">
  <img width="900" alt="Representative Performance" src="https://github.com/user-attachments/assets/7d51cb26-d461-441a-bd50-4b872b58ab18" />
</p>

<p align="center">
  <img width="900" alt="Product Performance Analysis" src="https://github.com/user-attachments/assets/46dc5387-32e8-4e68-bea7-1a3c9f2b1d9c" />
</p>

<p align="center">
  <img width="900" alt="Financial Payment Analysis" src="https://github.com/user-attachments/assets/6db4dedd-ba27-41c0-86c2-df1b5812bcce" />
</p>

---

## Example DAX KPIs & Measures

- Total Sales = SUM(Sales[Revenue])  
- Gross Profit = SUM(Sales[Revenue]) - SUM(Sales[Cost])  
- Collection Rate = DIVIDE(SUM(Payments[PaidAmount]), SUM(Sales[Revenue]))  
- Average Order Value = AVERAGE(Sales[OrderValue])

(These are illustrative — adjust names to match your model tables/columns.)

---

## Future Improvements

- Sales forecasting using time-series models  
- Customer segmentation (CLV / RFM) using ML techniques  
- Inventory and demand forecasting  
- Geographic sales heatmaps and territory optimization  
- Automated dataset refresh and deployment pipeline

---

## Related Analyses

### Netflix Content Trends & Strategic Analysis
Python | EDA | Pandas | Plotly | Seaborn

- Performed exploratory data analysis (EDA) on 7,700+ Netflix titles to uncover content strategy insights across genre, country, and rating.  
- Implemented a data preprocessing pipeline: column normalization, missing-value handling, duplicate removal, and date parsing.  
- Created interactive visualizations (choropleth maps, trend charts) to highlight regional content distribution and publishing trends.  
- Key findings example: Movies ≈69% of titles; U.S. and India are leading content-producing countries; TV-MA appears frequently among mature content.

Code, notebooks, and detailed analysis are available in the related repository(ies) — add the repo links here to point readers to the full notebooks and code.

---

## How to Use

1. Place the source dataset(s) in the `dataset/` folder or update the data source paths in Power BI.  
2. Open `Super Market Sales.pbix` in Power BI Desktop.  
3. Refresh the report to load data and recalculate DAX measures.  
4. Publish to Power BI Service for sharing and scheduled refresh (Pro/Workspace required).

---

## Author

**Katkam Sai Krishna** — Data Analyst | Power BI Developer | Python | SQL

Connect: [LinkedIn](https://www.linkedin.com/in/katkam-sai-krishna-aa4178302/) • Email: katkamsaikrishna2004@gmail.com

If you find this project useful, please ⭐ star the repository!
