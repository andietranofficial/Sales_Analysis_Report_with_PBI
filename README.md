# Sales Analysis Report with Power BI

## Architecture

```
Sales, target & product data (2020–2022)
        │
        ▼
Power BI data model ── DAX measures (Total Sales, Gross Margin, PY Sales,
        │                             % Growth, % of Target, Difference From Target)
        ▼
3-page "Sales Analytics" report
  ├── Overview            → KPIs, sales by store location & type, monthly trend
  ├── Sales vs. Target    → actuals vs. target & prior year, by quarter / store type / state
  └── Product Analysis    → top products, sales over time, CY vs. PY growth by department
        │
        ▼
Shared slicers: Year · Quarter · Location · Store Type · Department · Product
```

## Business Overview

Simple Store sells across 45 products, 5 departments and 3 store types (CORE, DIGITAL, LOCAL) in stores spread over US states. Managers need one place to see how sales are trending, which stores are hitting target, and which products drive revenue and margin. This report gives them that view across three linked pages, so they can move from a company-wide summary down to a single state, department or product without switching tools.

## Aim

Build an interactive Power BI report that tracks sales, gross margin and growth against target and prior year, and lets users slice performance by time, location, store type, department and product.

## Dataset Description

Store-level sales data covering 2020–2022. Key fields used in the report:

- **StoreID / Store Location** — store identifier and US state
- **Store Type** — CORE, DIGITAL or LOCAL
- **Department / Product / Product Type** — e.g. Clothing → Womens, Electronics → Tablets
- **Date** — rolled up to year, quarter and month
- **Sales** — sales amount
- **Target** — sales target per store
- **Gross Margin** — gross margin amount

## Approach

1. **Load and model the data** in Power BI, with a date dimension supporting year, quarter and month drill-downs.
2. **Create DAX measures** for Total Sales, Total Gross Margin, Average Margin, prior-year (PY) Sales, % Sales Growth, Total Target, Difference From Target and % of Target.
3. **Build the Overview page** — KPI cards, a map of sales by store location and type, monthly sales with growth, and sales by store type and department.

   ![Overview page](images/page%201.png)

4. **Build the Sales vs. Target page** — sales vs. PY and target cards, a quarterly sales-vs-target trend, a store-type comparison, and a state table with conditional formatting on sales and target gaps.

   ![Sales vs. Target page](images/page%202.png)

5. **Build the Product Analysis page** — sales by product type, top 5 products by sales and by gross margin, monthly sales by department, and a CY vs. PY growth matrix by department and product.

   ![Product Analysis page](images/page%203.png)

6. **Add navigation and slicers** — page buttons in the header and shared slicers so every page can be filtered the same way.
7. **Review the findings** — key insights and caveats from each page are written up in [dashboard-insights.md](dashboard-insights.md).

## Tech Stack

**Tool:** Power BI Desktop

**Language:** DAX

**Visuals:** KPI cards, map, clustered column, line and combo charts, donut chart, bar charts, matrix and table with conditional formatting
