# Supply Chain Analytics Platform | Power BI

## Overview

A multi-page Power BI analytics platform designed to provide end-to-end visibility into inventory, supplier performance, procurement, and delivery operations. The solution demonstrates data modeling, DAX, interactive dashboards, row-level security (RLS), and business intelligence best practices.

## Project Objectives

* Monitor inventory levels and stock value.
* Analyze supplier performance and ratings.
* Track order volumes across departments.
* Measure delivery performance.
* Enable department-specific access using Row-Level Security.
* Deliver interactive dashboards for executive decision-making.

## Dataset

The project consists of four related tables:

* **Inventory** – Product details, warehouse locations, stock levels, reorder levels, and unit costs.
* **Orders** – Procurement orders, suppliers, departments, quantities, and delivery times.
* **Suppliers** – Supplier information, regions, and ratings.
* **Calendar** – Date dimension for time intelligence.

Approximate dataset size:

* 100 Products
* 20 Suppliers
* 1,000 Orders

## Data Model

Relationships:

* Inventory (1) → Orders (Many)
* Suppliers (1) → Orders (Many)
* Calendar (1) → Orders (Many)

## Key DAX Measures

* Inventory Value
* Total Orders
* Total Quantity
* Average Delivery Time
* Fast Deliveries
* Slow Deliveries
* Low Stock Products
* Average Supplier Rating
* Dynamic Dashboard Title

## Dashboard Pages

### 1. Executive Dashboard

* KPI Cards
* Monthly Orders Trend
* Inventory by Category

### 2. Inventory Analytics

* Stock by Warehouse
* Stock by Product
* Reorder Analysis
* Inventory Value by Category

### 3. Supplier Performance

* Supplier Ratings
* Orders per Supplier
* Delivery Performance
* Supplier Region Distribution

### 4. Delivery Analytics

* Delivery Time Distribution
* Fast vs Slow Deliveries
* Monthly Delivery Trend
* Department Delivery Performance

### 5. Management Summary

* Executive KPIs
* Department Orders
* Supplier Rankings
* Category Breakdown

## Features

* Interactive slicers
* Dynamic DAX measures
* Conditional formatting
* Star-schema data model
* Row-Level Security (RLS)
* Scheduled refresh ready
* Cross-filtering visuals
* Department-based analytics

## Technologies Used

* Power BI Desktop
* DAX
* Power Query
* Microsoft Excel
* Power BI Service

## Business Value

This solution enables management to:

* Monitor inventory health.
* Identify low-stock products.
* Evaluate supplier performance.
* Compare departmental procurement activity.
* Track delivery efficiency.
* Support data-driven operational decisions.
