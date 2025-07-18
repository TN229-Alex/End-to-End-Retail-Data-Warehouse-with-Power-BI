# End-to-End Retail Data Warehouse with Power BI
This project showcases a business intelligence solution built using a simulated retail dataset. It includes a dimensional data warehouse design, data modeling using star schema, and an interactive Power BI dashboard for sales and inventory performance tracking.

## Tools & Technologies

- **SQL Server** for database modeling and ETL
- **Power BI** for data visualization
- **Dimensional Modeling** with star schema
- **DAX** for advanced metrics

## Data Warehouse Design

The data warehouse follows a galaxy schema model consisting of:

- **Fact Tables**:
  - Sales Fact
  - Inventory Fact

- **Dimension Tables**:
  - Date
  - Product
  - Customer
  - Sales Territory
  - Employee
  - Vendor
 
  ## Pipeline Architecture

![image](https://github.com/user-attachments/assets/c552d44e-ede2-4afd-97f3-3033242b77e5)

## SSAS Tabular Cube

This project includes a fully developed SSAS Tabular model (`Model.bim`) that was deployed to a local SSAS instance and connected to Power BI for high-performance reporting.

**Cube Features:**
- **Tables Imported From:** Warehouse.sql (Data Warehouse)
- **Modeling Tool:** SQL Server Data Tools (SSDT) for Visual Studio
- **Relationships Defined:** FactInternetSales → DimDate, DimProduct, DimCustomer, etc.

[`ssas_cube/`](ssas_cube) – contains the `.bim` cube model and project file.

 
  ## Power BI Dashboard

  This project includes an interactive Power BI dashboard built from the OLAP cube layer, enabling detailed insights into sales performance, regional trends and employee data.
  ![image](https://github.com/user-attachments/assets/dfec0d71-126c-4b0e-b564-88190240d471)

