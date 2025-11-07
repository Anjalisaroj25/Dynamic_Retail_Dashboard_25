# Dynamic Retail Dashboard in Excel
An interactive retail dashboard crafted in Excel—merging pivot tables, slicers, and charts to track KPIs like sales, stock, and regional performance. Designed for clarity and control, it turns spreadsheets into a strategic insights engine. 
## Overview
A dynamic retail dashboard in Excel is an interactive visual tool that tracks and analyzes key retail metrics—like sales, inventory, and customer behavior—using formulas, charts, slicers, and pivot tables. It allows users to filter data by region, product category, time period, and more.
## Datasets Used
### 1. Orders Table
The Orders table contains details of customer orders, including product, shipping, and financial metrics.
#### Sample Data:
### 📦 Sample Retail Orders Table

| Row ID | Order ID | Order Date | Ship Date | Ship Mode | Customer Name | Segment | Region | Category | Sub-Category | Product Name | Sales | Quantity | Discount | Profit |
|--------|----------|------------|-----------|-----------|----------------|---------|--------|----------|--------------|---------------|--------|----------|----------|--------|
| 1      | CA-2016-152156 | 11/08/2016 | 11/11/2016 | Second Class | Claire Gute | Consumer | West | Furniture | Bookcases | Bush Somerset Collection Bookcase | 261.96 | 2 | 0.0 | 41.91 |
| 2      | CA-2016-152156 | 11/08/2016 | 11/11/2016 | Second Class | Claire Gute | Consumer | West | Furniture | Chairs | Hon Deluxe Fabric Upholstered Chairs | 731.94 | 3 | 0.0 | 219.58 |
| 3      | CA-2016-138688 | 06/12/2016 | 06/16/2016 | Second Class | Darrin Van Huff | Corporate | West | Office Supplies | Labels | Self-Adhesive Address Labels | 14.62 | 2 | 0.0 | 6.87 |
### 2. Returns Table
Tracks orders that have been returned along with the associated markets.
#### Sample Data:
| BIS | Return Date | Product Code |
|-----|-------------|--------------|
| Yes | 02-Mar-2020 | AAMAM        |
| Yes | 03-Mar-2020 | AAPAM        |
| Yes | 04-Mar-2020 | AAPMC        |
| Yes | 05-Mar-2020 | AAPNC        |
| Yes | 06-Mar-2020 | AAPOC        |
| Yes | 07-Mar-2020 | AAPPC        |
| Yes | 08-Mar-2020 | AAPQC        |
| Yes | 09-Mar-2020 | AAPRC        |
| Yes | 10-Mar-2020 | AAPSC        |
### 3. People Table
Contains details about sales representatives and their respective regions.
#### Sample Data:
| Person         | Region     |
|----------------|------------|
| Anna           | America    |
| Chuck Williams | South      |
| Clay Mendez    | West       |
| Greg Collins   | East       |
| Julia Alvarez  | America    |
| Guleon Roberts | Caribbean  |
| Maria Smith    | Caribbean  |
## Problem Statements Solved with Steps
### 1. Key Performance Indicators (KPIs)
**Objective:** Calculate and display Total Sales, Total Profits, Total Quantity, Number of Orders, and Profit Margin dynamically.
##### Steps:
   1. Import the Orders Table into Excel using Power Query.
   2. Create calculated columns for:
       + Profit Margin = Profit/Sales
       + Total Orders = Count of Order ID
   3. Use Excel formulas to calculate:
       + Total Sales = =SUM(Sales)
       + Total Profit = =SUM(Profit)
       + Total Quantity = =SUM(Quantity)
   4. Build a dynamic KPI table and use symbols to enhance visual appeal.
 ### 📊 Business Performance Dashboard

![Dashboard Overview](dashboard.png)

