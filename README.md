## Project background
This project analyzes nearly 10,000 orders placed between 2014 and 2017 at a U.S. retailer of Technology, Office Supplies, and Furniture. Our objective is to uncover critical insights and recommendations across the business’s core drivers.

**Key Analysis Areas:**

- **Sales Trends Analysis:** Historical sales patterns, seasonal peaks, and volume fluctuations.
    
- **Product-Level Performance:** Revenue and margin comparisons across Technology, Office Supplies, and Furniture.
    
- **Customer Segment Profitability:** Profit contributions for Consumer, Corporate, and Home Office channels.
    
- **Regional & State Benchmarks:** Identification of top- and under-performing regions against national averages.
    
- **Promotion Effectiveness:** Impact of discounts on volume lift and margin erosion.
    
- **Shipping & Fulfillment Costs:** Profitability analysis by shipping mode.


## Data Structure Overview
The database consists of a single table with detailed information on every order. Each record captures order identifiers, dates, customer segment, product category, geography, shipping details, and financial metrics.

| Column Name   | Type    | Description                                                      |
| ------------- | ------- | ---------------------------------------------------------------- |
| Order ID      | String  | Unique identifier for each order                                 |
| Order Date    | Date    | Date when the order was placed                                   |
| Ship Date     | Date    | Date when the order was shipped                                  |
| Customer Name | String  | Name on the customer’s billing account                           |
| Segment       | String  | Customer segment: Consumer, Corporate, or Home Office            |
| Product Name  | String  | Name of the product sold                                         |
| Category      | String  | High‑level product group: Technology, Office Supplies, Furniture |
| Sub‑Category  | String  | More specific product line within each category                  |
| Sales         | Float   | Total dollar amount of the order                                 |
| Profit        | Float   | Dollar profit earned on the order                                |
| Quantity      | Integer | Number of units sold in the order                                |
| Discount      | Float   | Dollar amount discounted off the list price                      |
| Region        | String  | Business region (East, West, Central, South)                     |
| State         | String  | U.S. state where the order was shipped                           |
| Ship Mode     | String  | Delivery method used (Standard, First Class, Same Day, etc.)     |


## Executive Summary
From 2014–2017, 9,994 orders generated $2.29 M in sales, though widespread discounts on over half of transactions squeezed overall profit margins. The Home Office segment delivered the highest profit per order ($33.82), while Technology products accounted for 36.5% of revenue at a 17.4% margin. Expedited shipping options (First Class, Same Day) trimmed profits by up to 8%, and sales consistently peaked in November and December—prime windows for targeted promotions.

![Dashboard](Data/Dashboard.png)

**Customer Profitability:** Home Office $33.82 vs. Corporate $30.46 vs. Consumer $25.84. Corporate grew 12% in 2017 vs. 2016.
    
- **Promotion ROI:** Discounted orders spiked +20% volume in Nov–Dec but shrank margins from 15% to –2.9%.
    
- **Geographic Spread:** CA/NY/TX contributed 42% of total sales; ND/WV/ME <1%. Year‑over‑year CA grew 18%.
    
- **Product Mix:** Tech 36.5% revenue (17.4% margin), Supplies 31.3% (17.0%), Furniture 32.2% (2.5%). Furniture margin fell 30% in Q3 2016.
    
- **Logistics Impact:** Same Day orders held 12.5% margin vs. Standard Class at 12.1%, yet cost-per-order is 5% higher.
    
- **Seasonality:** Monthly peaks: Nov ($352K), Dec ($325K), Sep ($308K). Off‑peak Feb lows at $175K.

## Recommendations
Based on the findings from this project, the following actions are recommended:

- **Rethink blanket discounts:** With over 50% of orders including discounts and many of those turning a negative price cuts are doing more harm than good. Instead, shift to smart, seasonal or loyalty-based promotions that reward repeat customers and preserve margin.
    
- **Lean into Home Office and Corporate segments:** These customer groups consistently deliver stronger profits per order. Tailored offers, membership perks, or upsell bundles could encourage more frequent and larger purchases.
    
- **Invest in regional outreach:** California, New York, and Texas are clear strongholds. Maintain momentum in these states while testing low-cost, localized strategies in underperforming regions like North Dakota or West Virginia.
    
- **Simplify the product line:** Technology brings in both volume and margin, while Furniture lags behind. Reduce emphasis on low-margin SKUs and focus on bundling bestsellers to improve order size and return.
    
- **Rebalance shipping cost vs. experience:** Same Day and First Class delivery modes cut deep into profits. To keep them viable, introduce flat-rate fees or only offer them above a set order threshold.

## How to Use
1. Open `Dashboard.xlsx`.  
2. Go to **Data → Refresh All** to pull in/merge the latest [files](Dataset.xlsx).  
3. Navigate to the **Dashboard** sheet to interact with slicers and view KPIs.  
