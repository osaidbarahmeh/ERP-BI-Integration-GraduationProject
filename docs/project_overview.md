# Project Technical Overview

## 1. Business Context
The project was developed to solve inventory visibility and sales performance monitoring challenges in a multi-branch retail company.

Each branch operated independently with no centralized real-time inventory tracking, leading to:
- Manual inter-branch communication
- Delays in customer service
- Poor inventory planning
- Lack of analytical visibility

---

## 2. Proposed Solution

The solution integrates three main layers:

### Operational Layer
Implemented using Odoo ERP:
- Sales Module
- Inventory Module
- Purchase Module
- POS Integration

### Automation Layer
Implemented using n8n:
- Scheduled workflows
- Automated data synchronization
- Reorder alerts
- Purchase order suggestions

### Analytics Layer
Implemented using Power BI:
- Sales dashboard
- Inventory dashboard
- KPI monitoring
- Branch performance comparison

---

## 3. Data Modeling Approach

Two Star Schema models were implemented:

### Sales Model
FactSales  
Dimensions:
- DimProduct
- DimBranch
- DimDate

### Inventory Model
FactInventoryMoves  
FactStock  
FactTransfers  
Dimensions:
- DimProduct
- DimBranch
- DimDate

---

## 4. Key Business KPIs

- Total Sales
- Profit Margin
- Inventory Turnover Rate
- Stock Value
- Average Order Value
- Branch Performance

---

## 5. Business Impact

The system improved:
- Operational efficiency
- Inventory transparency
- Data-driven decision-making
- Branch performance monitoring
