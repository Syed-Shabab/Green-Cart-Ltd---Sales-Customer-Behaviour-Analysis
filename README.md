# Green-Cart-Ltd---Sales-Customer-Behaviour-Analysis
Q2 sales and customer behaviour analysis identifying £70k-£95k annual revenue opportunities through delivery optimisation and discount strategy refinement.

Project Overview:---

Business Intelligence analysis for Green Cart Ltd, a UK-based e-commerce company specializing in eco-friendly household products. The analysis integrated three datasets to uncover revenue patterns, customer behavior insights, and operational inefficiencies across Q2 2024.

Dataset: 2,998 orders, 30 products, 500 customers

Period: Q2 2024 (April-June)

Focus: Revenue drivers, discount effectiveness, customer lifetime value, delivery performance


<img width="991" height="474" alt="S2-9" src="https://github.com/user-attachments/assets/23e84087-6929-4b1d-b5b0-c4644402807b" />



Key Findings:--- 

Finding 1: Cleaning Products Dominate Revenue
Cleaning category generates £93,622 (39% of total revenue) with 3,584 units sold—double the second-place Storage category. Central and North regions drive 60% of Cleaning sales, indicating strong regional product-market fit.

Category Performance:

Cleaning: £93,622 (39%)

Storage: £46,931 (20%)

Outdoors: £40,063 (17%)

Kitchen: £33,934 (14%)

Personal Care: £24,917 (10%)



<img width="1014" height="569" alt="S2-1" src="https://github.com/user-attachments/assets/c954f224-ea40-4cf4-b22f-b01f81270763" />




Finding 2: Gold Customers Drive Disproportionate Value

Gold tier customers place 1,674 orders—2.5x more than Bronze and Silver combined—generating 30-35% of total revenue despite being the smallest segment. This indicates exceptional customer lifetime value in the premium tier.

Order Volume by Loyalty Tier:

Gold: 1,674 orders (highest engagement)

Silver: 659 orders (moderate)

Bronze: 625 orders (lowest)


<img width="994" height="580" alt="S2-4" src="https://github.com/user-attachments/assets/4731200c-c65c-4609-ac4e-b7072878c271" />


Finding 3: Critical Delivery Performance Crisis
40% of all orders experience delays, with East region worst at 42%. Delays affect all price bands equally (38-42%), indicating systemic logistics issues rather than product-specific problems. 298 orders flagged as underperforming (low quantity + high discount + delayed).

Regional Delay Rates:

East: 42% (worst performer)

North: ~40%

West: ~40%

Central: 39%

South: ~38%


<img width="689" height="402" alt="S2-5" src="https://github.com/user-attachments/assets/c6aa25ef-b618-43ee-abfd-a6786912ae0d" />


Finding 4: Discount Sweet Spot Identified

Medium discounts (10-20%) generate highest order quantities (3-4 items per order), while heavy discounts (>20%) show diminishing returns, reverting to 2-3 items per order. Current heavy discounting strategy is eroding margins without driving proportional volume.

Finding 5: 14-Day Conversion Window Critical

169 customers placed orders within 14 days of signup, showing immediate engagement. Customers who don't purchase in this window demonstrate significantly lower lifetime value, indicating a critical early activation period.

Business Impact :---

Revenue Opportunity: £70,000-£95,000 annually

1. East Region Logistics (+£15k-£20k)

-- Reduce delay rate from 42% to 35%

-- Recover lost sales from delivery issues


2. Discount Optimization (+£25k-£35k)

-- Eliminate heavy discounts (>20%)

-- Focus on 10-15% sweet spot

-- Protect margins while maintaining volume


3. New Customer Activation (+£30k-£40k)

-- Automated 14-day email campaign

-- 20-25% increase in first-purchase conversion

Data Cleaning Summary:---

Comprehensive cleaning performed across all three datasets to ensure analytical reliability:

1. Sales Data (2,998 records):

a) Standardized delivery_status from 6+ variations to 3 categories

b) Standardized payment_method and region fields

c) Converted order_date to datetime

d) Filled 517 missing discount values with 0.0

e) Removed 2 duplicate orders

f) Converted text quantities to numeric


2. Product Data (30 products):

a) Standardized text columns

b) Converted launch_date to datetime

c) Verified all product_ids unique


3. Customer Data (500 customers):

a) Standardized loyalty_tier from 7+ variations to 3 categories

b) Filled 22 missing values across multiple fields

c) Retained 2 "Unknown" customer_ids as separate entities

Result:--- Clean dataset with 98.5% completeness; 542 fields cleaned; 2 duplicates removed

Feature Engineering --

Created six analytical features to enable deeper business insights:

a) revenue - Net revenue after discounts (quantity × unit_price × (1 - discount))

b) order_week - ISO week number for time-series analysis

c) price_band - Categorized products as Low (<£15), Medium (£15-30), High (>£30)

d) days_to_order - Product age at purchase time

e) email_domain - Customer acquisition channel identification

f) is_late - Boolean flag for delayed deliveries

g) Additional features: discount_band, signup_month, consolidated region field

Tools Used:---

Python 3.8+ - Core programming language

Pandas - Data manipulation and cleaning

NumPy - Numerical operations

Jupyter Notebook - Interactive analysis

Matplotlib - Data visualization

Seaborn - Statistical visualizations

Business Recommendations:---

1. Priority 1: East Region Logistics Improvement

Address 42% delay rate through logistics partner review and route optimization. Expected 10-15% revenue increase in East region.

2. Priority 2: Implement 10-15% Discount Strategy

Focus promotions on optimal discount band; eliminate >20% discounts except clearance. Expected 5-8% margin improvement.

3. Priority 3: 14-Day New Customer Campaign

Launch automated email sequence for customers who haven't purchased within 14 days of signup. Expected 20-25% increase in first-purchase conversion.

Key Statistics:---

Total Revenue: £239,467 (Q2 2024)

Average Order Value: £79.91

Total Orders: 2,998

Customer Base: 500 customers

Product Catalog: 30 products across 5 categories

Overall Delay Rate: 40%

Top Category: Cleaning (39% revenue share)

Top Customer Tier: Gold (30-35% revenue contribution)



<img width="668" height="499" alt="S2-3" src="https://github.com/user-attachments/assets/5931e358-1d36-4302-ac2d-55e138dccde5" />


<img width="987" height="478" alt="S2-2" src="https://github.com/user-attachments/assets/feea4c30-38eb-4955-a883-db279e947829" />



<img width="819" height="570" alt="S2-8" src="https://github.com/user-attachments/assets/cdfb3ecd-d1bb-4bad-a489-b2bf2f3eee72" />





About :----

This project was completed as part of the UpTrail Business Intelligence Programme focusing on multi-dataset integration, feature engineering, and actionable business recommendations.

Charu Madaan

Data Analyst | QA Software Tester | Business Intelligence

Email: charumadaan88@gmail.com

LinkedIn: https://www.linkedin.com/in/charu-madaan-7100b2210/
