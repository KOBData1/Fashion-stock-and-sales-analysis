# Fashion-stock-and-sales-analysis
A data analytics case study exploring factors influencing product stock levels using Excel and Power BI. Includes data cleaning, exploratory analysis, and an interactive dashboard revealing insights on pricing, discounts, brands, and product types.

---

## Introduction
Retail businesses often struggle with balancing stock levels: some products sell out quickly, while others linger too long. To investigate the drivers behind stock availability, I analyzed a dataset containing product information, stock status, pricing, discounts, colors, brands, and product types. This case study covers the complete data journey from cleaning and exploratory data analysis (EDA) to dashboard design using Power BI.

--- 


## Dataset Overview
<img width="1000" height="300" alt="image" src="https://github.com/user-attachments/assets/a4a8ee58-a06a-4179-acd5-bcd2c495ad45" />

The dataset contained 15,000 rows of product listings with the following relevant columns:
- Product Type
- Brand
- Variant
- Price
- Dominant Color
- Compare-at Price
- Stock Status (In Stock, Out of Stock, Unknown)
 

---

## Data Cleaning (Excel & Power BI)
- Checked For Duplicates: There were no duplicate entries.
- Adjusted data types for all relevant columns to ensure smooth analysis later.
- Cleaned and standardized a messy Date column with mixed formats like 8/14/2019, 06-07-2019, etc., and changed them into MM-DD-YYYY.
- Handled Missing Values: Rows with missing key information were replaced with unknown.

  
  <img width="1000" height="300" alt="image" src="https://github.com/user-attachments/assets/3322b853-ba86-4cdb-b7fc-a41e43dc2503" />

  
- Created Calculated Fields in Power BI: % Discount: = (Compare-at Price - Variant Price) / Compare-at Price * 100.
 

<img width="1000" height="300" alt="image" src="https://github.com/user-attachments/assets/96fd7c39-dde6-4e69-9f14-af05e1e4b32f" />


 ---
 
## Exploratory Data Analysis (EDA)
### Business Question:
What influences product stock turnover? Does pricing, discount level, color, or brand affect how quickly products sell?
Key Insights:
- High Discounts Don’t Guarantee Sales: Products with 61%+ off were still largely in stock.
- Most Popular Brands & Colors Still in Stock: The most common 10 brands and 43 unique colors were also mostly in stock — popularity doesn’t necessarily mean faster turnover.

## Statistical Analysis
Weak Correlation with Price & Discount:
- Discount vs Stock Availability: -0.022.
- Variant Price vs Stock Availability: 0.040.
- Compare-at Price vs Stock Availability: 0.048.

  <img width="800" height="300" alt="image" src="https://github.com/user-attachments/assets/5b6ef22b-a044-4076-aff5-13d91c50033f" />

These weak correlations suggest pricing and discounts alone don’t significantly impact stock movement.

 
---
 
## Dashboard Design (Power BI)
Objective: Create an interactive dashboard to visualize stock distribution across product attributes and support inventory optimization decisions.

### Visual Elements:
- KPI Cards: Total In-Stock and Out-of-Stock Products.
- Bar Charts: Brand vs Stock Status (Top 10 Brands). Product Type vs Stock Status
- Column Charts: Stock status vs dominant color. Stock status vs discount range.
- Donut Chart: %Stock Status Distribution.
- Line chart: Sales Trend By Month.
- Slicers: Brand, Product Type, Discount Range, and Color.
- Navigation Buttons: Easy page transitions.
 

## Pages:
### Page 1 – Overview:

<img width="1000" height="540" alt="image" src="https://github.com/user-attachments/assets/c12dba3a-c459-4deb-a50c-3bd70c515460" />

##### Summary of stock status across discount ranges, brands, and product types.


### Page 2 – Stock Trends:


<img width="1000" height="540" alt="image" src="https://github.com/user-attachments/assets/69f6f3d0-0150-4398-a935-51f902593f20" />

##### Drilldown view exploring stock by color, top brands, and price-discount patterns.

 
---

## Key Insight for Stakeholders
- Despite high discounts, many products remain unsold.
- Popular brands and colors also linger in inventory, suggesting that popularity or price reductions alone don’t drive stock turnover.
- Sales Trend Analysis: Sales have shown consistent growth month-over-month — from 1.5k in June, to 4.1k in July, and 7.5k in August. This upward trend highlights potential seasonality or improved marketing during these months.

##### These insights point to the need for broader inventory strategies beyond pricing — such as bundling slow-moving items with bestsellers, improving marketing campaigns, or analyzing customer engagement and timing promotions around high-performing months.

 
---
 
## Recommendations
- Improve Product Positioning: Leverage targeted marketing campaigns to drive interest.
- Rethink Discount Strategies: Experiment with varying levels or time-based offers.
- Bundle Popular Items: Encourage turnover of slow stock by pairing with fast sellers.
- Investigate Consumer Behavior: Incorporate metrics like views, clicks, or cart abandonment.
- Refine Product Categorization: Ensure accurate classifications to enhance analytics.
 

 ---

## Conclusion
This project demonstrates how effective data analysis and dashboard storytelling can lead to actionable insights. The weak correlation between pricing/discount and stock turnover highlights the importance of considering alternative strategies like product positioning, bundling, and targeted promotions.

 
--- 

## Tools Used:
- Excel: Initial cleaning.
- Power BI: Calculated columns, DAX measures, visualizations, and dashboard creation.
 
##### Note: All calculated fields (like % Discount) and measures were created directly in Power BI using DAX.

 

(Link to Power BI file)[]
