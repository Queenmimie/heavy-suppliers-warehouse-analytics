Heavy Suppliers Warehouse Analytics & Operations Optimization

PROJECT TEAM & CONTRIBUTORS
Miriam Tom — Data Analyst / Repo Owner
Akintayo Bisola — Data Analyst ( Data Cleaning)
Shifau Ahmad_Data Analyst (Building insights, Pivot tables and pivot chart making) 


 Phase 1: Foundation & Exploration
🗓️ Week 1: Data Profiling & Initial Dataset Audit


 Executive Summary
Week 1 focuses on inspecting and auditing the Heavy Suppliers Warehouse Dataset. The primary goal is to perform initial data profiling, understand dataset schema, evaluate overall data quality, and documenting anomalies before performing full transformations in Week 2.

 Data Profiling & Quality Audit Summary

1. Dataset Dimensions & Attributes
Total Records Examined: Initial row count audit performed across primary warehouse tables.

Key Columns Identifiers: shipment_id driver id customer name date, revenue fuel cost, maintenance cost,miles driven primary freight type

2. Identified Data Anomalies & Quality Issues
During the initial profiling phase, the following operational and structural anomalies were flagged.


Currency Formatting: Text characters and currency symbols ($) present in financial metrics (revenue fuel_cost maintenance_cost), requiring conversion to numeric floats.
Missing/Null Values: Blank/null records identified across operational cost fields requiring contextual imputation.

Redundant Records: Potential duplicate transaction logs flagged across unique shipment keys.


 Data Dictionary (Initial Draft)

Column Name | Raw Data Type | Expected Data Type | Description & Notes 
shipment_id Text, Text, Key | Unique tracking code per warehouse dispatch 
customer_name, Text, Text, Primary
primary_freight_type, Text, Categorical  Cargo classification.
revenue, Text, Numeric (Float)  Gross freight charges generated ($ USD)
fuel_cost, Text String, Numeric (Float) | Transport fuel expenditure
maintenance_cost, Text,String, Numeric (Float) Vehicle upkeep, servicing expense,
miles driven, Integer,Numeric, Total route distance traveled


Deliverables Posted
raw_heavy_suppliers_warehouse_dataset.csv: Uncleaned operational log file.
