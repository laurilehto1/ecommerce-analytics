# E-Commerce Analytics Project | Data Modeling & Power BI
**PostgreSQL + Power BI + DAX**

## Overview
This project demonstrates an end-to-end Business Intelligence pipeline using a Brazilian e-commerce dataset. Raw relational data is transformed into structured business insights through SQL-based preparation, star schema modeling, and KPI-driven dashboard design.

## Data Source
The dataset used in this project is the **Brazilian E-Commerce Public Dataset by Olist**, publicly available on Kaggle.  

Source: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce  

## Tech Stack
- **PostgreSQL** – data storage, relational modeling, SQL transformations  
- **Power BI** – star schema data model, relationships, interactive dashboards  
- **DAX** – business KPI calculations  


## Data Architecture
**Pipeline:**  
PostgreSQL (raw tables + views)  
→ Power BI (data model + relationships)  
→ DAX measures  
→ Dashboard visuals + insights  

**Model Design:**  
- Fact tables: `orders`, `order_items`, `order_payments`  
- Dimension tables: `CustomersDim`, `products`  
- One-to-many relationships  
- Cardinality issue resolved by creating `CustomersDim` with unique `customer_id`


## Key KPIs
- Total Revenue  
- Total Orders  
- AOV (Average Order Value)  
- Delay Rate  
- Avg Delivery Days  
- Total Payment Value  
- Avg Payment per Order  

All KPIs are implemented as reusable DAX measures and used consistently across visuals.


## Business Questions Answered

### Commercial
- How has revenue evolved over time?  
- Which states generate the most revenue?  
- Which product categories drive performance?  

### Operational
- Where are delivery delays concentrated?  
- Does delay rate correlate with revenue growth?  
- What payment methods dominate transaction value?  
