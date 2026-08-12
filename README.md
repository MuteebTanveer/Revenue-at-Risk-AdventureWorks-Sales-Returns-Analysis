# Revenue at Risk: AdventureWorks Sales & Returns Analysis

## Overview
A Power BI case study analyzing 3 years (2020–2022) of AdventureWorks sales data — approached as a Business Analyst investigating a business problem, not just building another dashboard. The goal was to answer the questions a CEO would actually ask, not just report revenue by month.

## Business Questions Investigated

**Revenue Health**
- Is revenue growth sustainable?
- Which products, categories, territories, and months have the highest return rate?

**Product Performance**
- Which products generate the most revenue?
- Which products generate revenue but also create costly returns?
- High sales + low return, high sales + high return, low sales + high return — which products fall where?

**Territory Performance**
- Which territories generate the highest and lowest revenue?
- Which territories deserve more investment — and which need attention?

**Discount Strategy**
- Are we rewarding the right products with discounts?
- Are discounts actually increasing sales?
- Which category has the highest discount rate?

## Key Findings

- Revenue grew 45.6% from 2020 to 2021 ($6.4M → $9.32M), then plateaued in 2022 (-1.5%, $9.19M)
- Road Bikes declined 26.6% year-over-year — hidden inside an overall "flat" 2022 number, while Touring Bikes grew 70% in the same period
- $765,277.84 in revenue lost to returns across 3 years
- Return rate stayed stable (3.27% → 2.13% → 2.15%) even as raw return volume grew (86 → 770 → 972 units) — the return problem is scaling with the business, not outpacing it
- Discount level doesn't correlate with returns at the yearly/company level — but at the individual product level, low-volume bike models with heavy discounts (avg 18.3%) return at rates up to 11.8%, compared to under 2% for high-selling, low-discount accessories
- Mountain-200 (Black/Silver) became the top-performing model from 2021 onward, replacing Road-150 which led in 2020
- Australia and the United States are the top two revenue-generating markets, followed by UK, Germany, France, and Canada

## Product Segmentation

Classified every product into 4 groups based on sales volume and return rate:
- **High Sales, Low Return** — star performers (Water Bottle, Patch Kit, Tire Tubes, AWC Logo Cap)
- **High Sales, High Return** — watch list (Sport-100 Helmets, HL Tires, Hydration Pack)
- **Low Sales, High Return** — biggest risk (Road-650 Red, Touring-2000, Mountain-100/500 variants) — all heavily discounted, low-volume bike models

## Tools & Techniques

- **Power BI** — report design, relational data modeling
- **DAX** — SUMX, CALCULATE, RANKX, ALLEXCEPT, dynamic filter context, SWITCH-based segmentation
- **Data Modeling** — multi-table relationships (Sales, Returns, Product, Territory, Discounts, Calendar), resolved relationship ambiguity and many-to-many issues
- **Visualization** — treemaps, decomposition tree, geographic maps, log-scale scatter analysis, dual-axis comparisons

## Report Structure (3 Pages)

1. **Sales Performance** — Revenue trends, top products, category breakdown, territory map
2. **Returns & Revenue Impact** — Return rate by month/year, revenue lost to returns, most-returned products by continent
3. **Discount & Risk Analysis** — Discount rate by category, product segmentation scatter chart, sales-return risk classification

## File

`AdventureWorks_Revenue_Risk.pbix` — open in Power BI Desktop to explore interactively (drill-through, slicers, cross-filtering across all pages)
