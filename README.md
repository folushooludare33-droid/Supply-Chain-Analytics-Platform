# Supply Chain Analytics Platform | Power BI

A comprehensive multi-page Business Intelligence solution built with Power BI to provide end-to-end visibility across inventory, procurement, supplier performance, and delivery operations. The project demonstrates modern BI development practices through dimensional data modeling, Power Query transformations, DAX calculations, Row-Level Security (RLS), and interactive dashboards that support operational and executive decision-making.

Designed using a star-schema model, the platform enables stakeholders to monitor supply chain performance, identify operational bottlenecks, evaluate supplier reliability, and optimize inventory management through data-driven insights.

---

## Features

### Executive Analytics

* Executive KPI Dashboard
* Company-wide operational overview
* Interactive business summaries
* Monthly procurement trends
* Inventory performance monitoring
* Executive-level reporting

### Inventory Management

* Inventory Value Analysis
* Warehouse Stock Monitoring
* Product Stock Levels
* Low Stock Alerts
* Reorder Level Analysis
* Inventory Distribution by Category

### Supplier Performance

* Supplier Rating Analysis
* Supplier Performance Rankings
* Procurement Volume by Supplier
* Regional Supplier Distribution
* Delivery Performance Monitoring
* Supplier Comparison Dashboard

### Procurement Analytics

* Total Orders
* Purchase Quantity Analysis
* Department Procurement Activity
* Monthly Order Trends
* Category Purchasing Analysis
* Order Distribution Reports

### Delivery Performance

* Delivery Time Analysis
* Fast vs. Slow Deliveries
* Department Delivery Metrics
* Monthly Delivery Trends
* Delivery Performance Distribution

---

## Business Intelligence Architecture

```text
Excel Data Sources
        │
        ▼
Power Query
(Data Cleaning & Transformation)
        │
        ▼
Star Schema Data Model
        │
        ▼
DAX Measures & Calculations
        │
        ▼
Interactive Power BI Dashboards
        │
        ▼
Executive Decision Making
```

---

## Dataset

The project uses four related datasets representing a simplified supply chain environment.

### Inventory

Contains:

* Product ID
* Product Name
* Category
* Warehouse
* Stock Level
* Reorder Level
* Unit Cost

### Orders

Contains:

* Order ID
* Product ID
* Supplier ID
* Department
* Quantity
* Order Date
* Delivery Date
* Delivery Time

### Suppliers

Contains:

* Supplier ID
* Supplier Name
* Region
* Supplier Rating

### Calendar

Provides:

* Date
* Month
* Quarter
* Year
* Time Intelligence Support

---

## Data Model

The solution follows a star-schema model with clearly defined one-to-many relationships.

```text
Calendar
    │
    ▼
 Orders
 ▲      ▲
 │      │
Inventory  Suppliers
```

Relationships:

* Inventory (1) → Orders (Many)
* Suppliers (1) → Orders (Many)
* Calendar (1) → Orders (Many)

---

## Power Query Transformations

The project includes several data preparation steps:

* Data Type Conversion
* Null Value Handling
* Column Renaming
* Calculated Columns
* Data Cleaning
* Relationship Preparation
* Calendar Table Creation

---

## DAX Measures

The report includes dynamic DAX calculations such as:

* Inventory Value
* Total Orders
* Total Quantity Ordered
* Average Delivery Time
* Fast Deliveries
* Slow Deliveries
* Low Stock Products
* Average Supplier Rating
* Dynamic Report Titles
* KPI Calculations

---

## Dashboard Pages

### Executive Dashboard

Provides an executive overview including:

* KPI Cards
* Monthly Orders Trend
* Inventory by Category
* Procurement Overview
* Executive Summary Metrics

### Inventory Analytics

Includes:

* Stock by Warehouse
* Stock by Product
* Inventory Value
* Low Stock Analysis
* Reorder Monitoring

### Supplier Performance

Displays:

* Supplier Ratings
* Supplier Rankings
* Orders per Supplier
* Regional Distribution
* Delivery Performance

### Delivery Analytics

Contains:

* Delivery Time Distribution
* Fast vs. Slow Deliveries
* Monthly Delivery Trends
* Department Performance

### Management Summary

Provides:

* Executive KPIs
* Department Orders
* Supplier Rankings
* Category Performance
* Operational Summary

---

## Power BI Features Demonstrated

* Star Schema Modeling
* Power Query
* Data Transformation
* DAX Measures
* KPI Cards
* Interactive Slicers
* Drill-Down Analysis
* Cross-Filtering
* Conditional Formatting
* Time Intelligence
* Dynamic Titles
* Bookmarks
* Row-Level Security (RLS)
* Scheduled Refresh Configuration

---

## Technologies Used

* Microsoft Power BI Desktop
* Power BI Service
* DAX
* Power Query
* Microsoft Excel

---

## Project Structure

```text
Supply-Chain-Analytics-Platform/
│
├── data/
│   ├── Inventory.xlsx
│   ├── Orders.xlsx
│   ├── Suppliers.xlsx
│   └── Calendar.xlsx
│
├── reports/
│   └── Supply_Chain_Analytics.pbix
│
├── screenshots/
│   ├── executive_dashboard.png
│   ├── inventory_dashboard.png
│   ├── supplier_dashboard.png
│   ├── delivery_dashboard.png
│   ├── management_summary.png
│   ├── data_model.png
│   └── rls_configuration.png
│
└── README.md
```

---

## How to Use

1. Open the `.pbix` file using Power BI Desktop.
2. Refresh the data model if required.
3. Navigate through the five dashboard pages.
4. Use slicers to filter data by supplier, warehouse, department, or date.
5. Explore KPIs and visualizations.
6. Test Row-Level Security using the **View As** feature.

---

## Business Reports Generated

The platform provides insights including:

* Executive KPI Dashboard
* Inventory Health Report
* Supplier Performance Report
* Procurement Analysis
* Delivery Performance Dashboard
* Department Procurement Summary
* Inventory Value Report
* Low Stock Monitoring
* Supplier Rankings
* Monthly Operational Trends

---

## Skills Demonstrated

* Business Intelligence
* Power BI Development
* Data Modeling
* Star Schema Design
* DAX
* Power Query
* Data Transformation
* Dashboard Design
* KPI Development
* Row-Level Security (RLS)
* Interactive Reporting
* Supply Chain Analytics
* Data Visualization
* Executive Reporting

---

## Screenshots

Store screenshots inside the `screenshots/` folder.

### Executive Dashboard

```text
screenshots/executive_dashboard.png
```

### Inventory Analytics

```text
screenshots/inventory_dashboard.png
```

### Supplier Performance

```text
screenshots/supplier_dashboard.png
```

### Delivery Analytics

```text
screenshots/delivery_dashboard.png
```

### Management Summary

```text
screenshots/management_summary.png
```

### Data Model

```text
screenshots/data_model.png
```

### Row-Level Security

```text
screenshots/rls_configuration.png
```

---

## Business Value

Modern supply chains generate large volumes of operational data that must be transformed into actionable insights. This Power BI platform consolidates inventory, procurement, supplier, and delivery information into a centralized analytics solution, enabling managers to monitor stock health, identify procurement trends, evaluate supplier performance, and improve delivery efficiency. By combining interactive dashboards, DAX calculations, and Row-Level Security, the solution supports informed decision-making while ensuring secure access to department-specific information.

---

## Future Improvements

* Real-time ERP integration
* Predictive inventory forecasting
* Supplier risk scoring
* Demand forecasting with machine learning
* Inventory optimization recommendations
* Purchase order approval workflow
* Automated email alerts
* Mobile-optimized dashboards
* AI-powered anomaly detection
* Integration with Azure SQL and Microsoft Fabric

---

## Author

Developed as a portfolio project demonstrating Power BI development, business intelligence, dimensional data modeling, DAX programming, dashboard design, supply chain analytics, and executive reporting.
