# E-Commerce User Journey & Funnel Analysis

## 🎯 Project Objective
- Why do thousands of users add products to their carts but never complete the purchase?
- At which stage of the customer journey—browsing, adding to cart, or checkout—are users lost the most? 
- Which product categories drive revenue and which face the highest drop-offs?

In this project, I analyze an e-commerce dataset of 1 million events to map the user journey from product views to purchases using conversion funnels, drop-off analysis, and heatmaps. The goal is to uncover actionable insights that help businesses optimize product offerings, reduce cart abandonment, and improve overall user engagement.

---

## 📂 Dataset Information
- *Source:* Kaggle/Public Dataset eCommerce behavior data from multi category store
- *Dataset Link:* https://www.kaggle.com/datasets/mkechinov/ecommerce-behavior-data-from-multi-category-store
- *Rows Used:* 10 lakh rows for analysis  
- *Columns:* event_time – Timestamp of the event, event_type – Type of event (view, cart, purchase), product_id – Unique product identifier, category_id – Category ID, category_code – Category hierarchy (main.sub.subsub), brand – Product brand, price – Product price, user_id – Unique user identifier, user_session – Session identifier  
- *Description:* This dataset contains behavior data for 2 months (from October 2019 to November 2019) from a large multi-category online store. Each row in the file represents an event. All events are related to products and users. Each event is like many-to-many relation between products and users.

---

## 🛠 Analysis Steps
1. Data Cleaning
   - Removed duplicates  
   - Handled missing values for category_code, brand, and category_id  
   - Standardized event_time and extracted features: event_hour, event_month, is_weekend  

2. Exploratory Data Analysis (EDA)
   - Count of event types  
   - Top categories, sub-categories, brands, and products  
   - Price distribution (histogram & boxplot)  
   - Repeat customer purchases  
   - Time-based analysis by hour, weekday/weekend, and month  

3. Conversion Funnel & Drop-Off Analysis
   - Conversion rates between view → cart → purchase  
   - Category-wise drop-off percentages  

4. Revenue Analysis
   - Top categories by revenue  
   - Pareto analysis  

---

## 📊 Analysis & Key Visualizations
### 1. Event Type Distribution
- Majority of events are *views, followed by **purchases* and *cart additions*.  

### 2. Top Categories by Count
- Electronics and smartphones dominate user interactions; *unknown categories* also have high event counts.  

### 3. Top Brands
- Samsung, Apple, and Xiaomi lead in user engagement.  

### 4. Price Distribution
- Most products are priced between *0–500. Outliers extend up to **2200*.  

---

## 🔑 Insights & Key Findings
- *Event Funnel:* Highest conversion occurs at *cart → purchase; major drop-offs occur at **view → cart* stage.  
- *Top Revenue Categories:* Electronics generate the most revenue, while smaller categories cumulatively reach 100%.  
- *Repeat Customers:* Few users contribute to multiple purchases, highlighting loyalty potential.  
- *Time Patterns:* Peak purchase hours are *4–8 PM*; weekend impact is limited due to only two weekend days in dataset.  

---

## 💡 Business Recommendations
- Improve *checkout flow* to reduce cart → purchase drop-offs.  
- Target marketing and promotions for *high cart but low purchase categories*.  
- Focus on *high-revenue categories* like electronics for campaigns and bundles.  
- Design *loyalty programs* for repeat customers to increase retention.  

---

## 📌 Conclusion
This project analyzes *10 lakh rows of e-commerce data* to reveal patterns in user behavior from *views to purchases*.  
By combining *conversion funnels, category-level insights, and revenue analysis*, businesses can identify bottlenecks, optimize conversions, and increase revenue in a structured and actionable way.
