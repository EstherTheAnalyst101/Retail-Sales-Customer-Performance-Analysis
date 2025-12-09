# Retail-Sales-Customer-Performance-Analysis
The objective of this project is to present a comprehensive analysis of sales performance across products, customers, regions and countries. This is to identify growth using Power BI. KPI's were achieved through data cleaning, transformation and visualization
# 1. Project Overview
**Retail Sales, Product and Customer Dataset**  (ID, Order date, Name, Year, Category, Sub category, Loyalty status, Country, Gender, Age, Supplier, Region, Discount, Quantity). 
The objective is to create an interactive Sales Analysis Dashboard in Power BI that answers;
*	Which product generates the most revenue?
* Which country contributes most to revenue?
*	Who are the top customers and what drives their loyalty?
* How does sales trends vary by region, category and time?
* Which product category contributes most to growth?
# 2. Data Understanding
*The following datasets were used:
	Sales - data.csv – transactional sales records
	Product – data.xlsx – product details
	Retail – sales_dataset.csv – supporting data on customer and transaction details.
* Key fields: Transaction ID, Order date, Name, Year, Category, Sub category, Loyalty status, Country, Gender, Age, Supplier, Region, Discount, Quantity.
* Limitations: The sample size was small, there were missing values.
  
# 3. Methodology
## i.Data Cleaning (Power BI)
*	Removed unnecessary columns, duplicate IDs, blank fields, and inconsistencies.
*	Formatted columns:
  Dates ↔ Date format
	Price / Cost ↔ Currency format
* Handle missing values: Replaced with unknown or average where applicable
* Renamed columns for clarity (eg. CustID ↔ Customer ID)
* Merged Queries:
	Merged Sales with Products on Product ID
	Merged sales with customers on Customer ID
## ii.Feature Engineering (Power Query Editor)
* Added calculated columns(DAX):
  * Discount % = Discount / 100
  * M.Revenue = Quantity * Unit price
  * Discount Amount = Discount% * M.Revenue
  *  Net Revenue = M.Revenue - Discount Amount
## iii. Visualization(Power BI)
 * Dashboard 1: Overview of Sales Performance
 * Dashboard 2: Product Overview
*  Dashboard 3: Sales Overview

   # 4.The Dashboards




<img width="1331" height="732" alt="image" src="https://github.com/user-attachments/assets/b8200174-69c2-4cf1-a8aa-d557f8721e65" />



















   

 # Overview of Sales Performance
* **Total Revenue**: 106.44K
* **Total Stock**: 220 units
* **Total Discount Amount**: 14.00K
* **Total Orders**: 50
## Revenue by Region
*	Regional sales are fairly balanced, but North and East remain the strongest markets contributing 29.39K and 28.00K to revenue respectively.
*	**North** leads with the highest revenue, followed closely by East.
*	West and South contribute slightly lower but still significant sales volumes with 25.45K and 23.60K respectively.
## Revenue by Product Category
* **Furniture** dominates revenue generation with 65.44K showing high-value sales possibly driven by larger ticket items.
*	Clothing follows with 22.59K of total revenue and Electronics (18.41K) at much lower levels, signaling a product mix imbalance
  ## Monthly Revenue Trend
* Revenue is modest from January to March
* **April** emerges as a standout month, suggesting either seasonal demand or effective promotions during that period.
*	A strong peak in **April (35.46k)** indicates major demand acceleration, followed by a gradual decline into **June(21.38K)**
  ## Revenue by Gender
*	**Male shoppers dominate revenue** contribution,**highlighting an untapped opportunity in female market engagement.**
* **Male customers drive 90.9%** of total revenue
 * **Female customers represent only 9.1%,** showing a major demographic skew





<img width="1335" height="727" alt="image" src="https://github.com/user-attachments/assets/1f3cc989-48de-4b88-b8c1-12cc923528ab" />














 #  Product Overview
* **Top Product by Revenue**: Product 12 – 14.3K
* **Top Sub-Category by Revenue**: Laptop – 29.9K
* **Top Category by Revenue**: Furniture – 65.4K
*  **Top Supplier by Revenue**: Supplier A - 44.7K

## Quantity Distribution by Product Category
* **Furniture which is the leading category** accounts for **59% of total units sold (130 units)**
*   Clothing contribute 22% (49 units) and Electronics also contributes 19% (41 units), indicating uneven demand spread
  * **Laptop segment is a major revenue and quantity driver**, reflecting strong consumer interest in technology-related products.

 ## Quantity Trend by Month
* **Monthly sales trend is positive, peaking in April – May** relate to promotional campaigns or seasonal demand.
* **Sales picked up steadily** from January (27) to a peak in April (53)
*  Slight drop but still strong performance in May (42) and June (41)
 ## Regional Revenue
*	Sales are fairly consistent across regions, with only minor variance, implying balanced market coverage.
* **Strongest markets: North (29K) and East (28K)**
* **West (25K) and South (24K) show potential but lag slightly behind**






<img width="1331" height="723" alt="image" src="https://github.com/user-attachments/assets/221207f9-4ea5-4c97-ab18-4870ff18b3bd" />















  
# Customer Overview
## Top Performers
* **Top customer by Revenue**: Customer1 generating 20.4k of total revenue
* **Top country by Customer**: France emerged the top performing country by customer.
* **Top status by Customer count**: Bronze with 8 counts
## Count of Loyalty by Loyalty Status
The customer base consists primarily of **Bronze-tier customers** with a strong revenue concentration in a few key individuals and countries. **Bronze recorded the highest count by loyalty status of 8.**       Followed by **Gold**and **Silver** recording a count of 6 each.
## Total revenue By Gender and Age
 Most customers are **middle-aged and male**, contributing to the **majority of revenue**. The **average customer age is 38**.
## Number of Customers by Country
 Geographic performance is uneven, with **UK** showing clear dominance in both **revenue and customer presence**, while other regions recorded low customer base.
 This profile highlights potential to increase customer value through loyalty growth, gender-balanced engagement, and broader regional expansion.


# 5.Key Insights
## Sales Insights
* **High-value categories like Furniture generate the most revenue**, showing strong pricing and demand power.  This category controls the majority of quantity sales, suggesting market concentration and product dependency. However, over reliance on Furniture as the main revenue engine may increase concentration risk.
* **Laptop sub-category is a major revenue and quantity driver**.  It performs strongly, indicating a strong presence and demand in tech-driven products.
* **Monthly sales trend is positive**, peaking in April – May relate to promotional campaigns or seasonal demand.
* Sales are fairly consistent across regions, with only minor variance, implying balanced market coverage.
* Supplier A is a key revenue driver, indicating valuable supplier partnership and potential reliance.
## Demographic Insights
* Gender Distribution:
There is a **significant gender imbalanced** in customer purchasing behavior with **Males representing 90.9%** of total revenue (96.75k) and **9.1% for females representing (9.68k)** of total revenue, indicating the need for gender specific market dominance.
* Age Distribution:
Customers range from **young adults to middle-aged individuals**, with most falling between ages of **30–55**.
This highlights a mature and potentially stable customer base.
## Geographic Insights
* **Customers** are primarily from a number of countries, including the **France, UK, USA, Canada and Germany.**
* **UK**appears to have the highest representation, suggesting it may be the company’s strongest market or most accessible demographic segment.
* Geographic concentration may influence loyalty tier distribution markets with higher participation show greater loyalty. 
*	**The North region outperforms all others with $29k in revenue** with the **south region contributing the least revenue $24k.**
*	Regional revenue is relatively balanced with North and East outperforming.
## Loyalty Insights
*	Customers fall into different loyalty tiers: **Bronze, Silver, and Gold.**
*	**Bronze status appears more frequently**, which indicates a **good proportion** of highly engaged or repeat customers.
* However, there remains room to **elevate Gold and Silver customers into higher tiers** through targeted engagement.
* The combination of age and loyalty tier suggests **older customers tend to hold higher loyalty statuses.**
  
# 6. Recommendations
 * **Investigate the South and West regions** for barriers such as distribution issues, low brand visibility, or pricing concerns.
 *	Launch region **targeted marketing and promotional campaigns** to boost sales. 
 *	**Expand the furniture product line** or introduce premium product versions.
 *	Evaluate whether **discounts are improving order volume or simply reducing margins.**
 *	**Shift to value added promotions** instead of blanket price reductions.
 *	Use **demographic and loyalty data** to build customized communication strategies that reflect unique customer needs.

# 7. Conclusion
This project shows how structured analysis of Sales, Product, and Customer data using **Power BI** can generate clear business insights.
Overall, **Sales is doing well,** with strong order value, balanced regional penetration, and a clear product category leader. **Product performance is solid,** with strong demand for key categories and stable sales coverage across regions. There is a **stable customer base with an imbalanced demographics with males dominating** the demographics, strong representation from specific regions, and a promising distribution of loyalty tiers.
It demonstrates end-to-end analytics workflow.

# 8. Tool; Power BI & skills demonstrated
*	Data Cleaning & Transformation
*	Data modelling and Analysis
*	Interactive slicers & Timelines
*	Dashboard design & Visualization
*	Business reporting
