# Retail Sales Performance Dashboard

**Tools:** Excel (XLOOKUP, VLOOKUP, PivotTables, Slicers)
**Full write-up:** https://achieved-flannel-c99.notion.site/Sales-Performance-Dashboard-Retail-Analysis-3e3b332e9de2816d8cf5caff349f63fd (Notion case study)

## Overview
Consolidated three separate raw tables — Transactions (9,749 rows), Customers (9,995 rows), and Products (1,691 rows) — into a single clean dataset of 8,413 rows, then built an interactive sales dashboard filterable by Segment, Region, Category, and Year.

## Key Findings
- Technology is the top-selling category ($3.27M), ahead of Furniture ($2.37M) and Office Supplies ($2.15M)
- Standard Class shipping accounts for ~60% of all orders (2,915 of 4,885)
- Sales spike sharply in November and December ($1.16M and $1.08M) versus a ~$580K average across other months — a holiday-season pattern
- West region moves the highest volume (10,651 units), while Central holds a slightly stronger average profit margin

## Methodology
1. Pulled Customer Name, Segment, and Region into the transaction table via `XLOOKUP`
2. Pulled Price and Cost per product via `VLOOKUP`
3. Calculated Sales (Price × Qty), Cost (Cost × Qty), Profit (Sales − Cost), and Profit Margin (Profit ÷ Sales)
4. Built PivotTables and a dashboard with Segment/Region/Category/Year slicers

## Files
- `sales_dashboard.xlsx` — full workbook (raw tables, cleaned data, pivots, dashboard)
- `dashboard_screenshot.png` — dashboard preview
