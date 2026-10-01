# Sales Analytics Dashboard — Key Insights

Source: Simple Store "Sales Analytics" Power BI report, 3 pages (Overview, Sales vs. Target, Product Analysis).

## Page 1: Overview

- **Scale:** Total Sales 4,048M, Total Gross Margin 2,221M — margin is about 55% of sales, matching the "Average of Margin" card.
- **Footprint:** 3 store types, 5 departments, 45 products.
- **Store type:** CORE has the biggest map bubbles and by far the highest sales (~1,000M in the Store Type/Department chart), well ahead of DIGITAL and LOCAL.
- **Department leader:** Clothing leads within CORE.
- **Seasonality:** November has the highest monthly sales (~480M). Growth (the line) peaks in May (~65%) and dips in June (~41%) — growth and sales volume don't move together.
- **Trap:** the sales-growth line uses a right-hand axis that starts around 40%, not 0% — its swings look larger than they are next to the sales bars.

## Page 2: Sales vs. Target

- **Headline:** Sales are 1,387.16M — +10.01% vs. target (1,261M) and +4.17% vs. prior year (1,331.59M). Beating target is the bigger story than beating last year.
- **Trend:** Sales and target lines track closely through 2020–early 2021; the gap widens most by late 2022.
- **Store type:** CORE has the largest absolute gap between sales and target of the three store types.
- **State performance:** Table sorted by Total Sales, with % of Target and Difference From Target columns. West Virginia (94% of target) and Oklahoma (96%) are among the states under 100%, despite being high on the sales list.
- **Trap:** the status icons (green tick / amber / red cross) follow the Total Sales ranking, not % of Target — West Virginia gets a green tick at 94% of target, while Oregon gets a red cross at 114% of target. Icon thresholds shift with whatever filter is applied.

## Page 3: Product Analysis (filtered to Alabama)

- **Context:** page is filtered to Location = Alabama; other slicers (Store Type, Department, Product) are set to All.
- **Product mix:** the product-type donut and the "Top 5 Products With Best Sales" and "Top 5 Products With Best Gross Margin" charts show the same five products in the same order (Books, Assorted Food, Appliances, Kitchens, Womens) — margin appears to track sales volume closely.
- **Growth by department (CY vs PY):** Clothing +46%, Electronics +38%, Garage +45%, Kitchen +45% (visible rows; table scrolls further).
- **Trap:** "Misc" (under Clothing) shows +132% growth, but on a small base (~9.8K vs ~4.2K); Desktops shows −11% on ~73 vs ~82 units. Large percentage moves on small bases can be misleading — always check the absolute value behind a percentage.
- **Sales Overtime chart:** monthly pattern by department, with "Other" as the largest series — worth digging into what departments/products that bucket contains.


