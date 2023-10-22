# Sales-Data-Warehouse
# Building-Sales-Data-warehouse-Using-ETL-SSIS-SQL SERVER

## Overview:
By using [AdventureWorks2014](https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorks2014.bak) Dataset I have built a Sales Data Mart using (SQL Server Integration Services SSIS) SQL Server involves leveraging the capabilities of Integration Services (SSIS) and the Modeling of SQL Server, This Data mart offers several benefits, making them valuable components in the main purpose of data management and analytics within organizations

## Technologies:
* Visual Studio
* SQL Server Integration Services (SSIS)
* SQL Server Management Studio (SSMS)

## Project Stages

**1- Data Extraction:** 


* Using SQL Server Integration Services (SSIS), we extracted relevant data from the AdventureWorks2022 database. This extraction process involved identifying essential tables and fields for analysis.

**2- Data Preprocessing:**

  
* To ensure data quality and accuracy, we performed data cleansing and preprocessing tasks. This step involved handling missing values, removing duplicates, and transforming data as needed.

**4- Star Schema Design:**


* The foundation of our data mart is the star schema. We meticulously designed this schema to align with the specific analytical requirements of our project. This schema includes dimension tables describing various attributes and a central fact table containing numerical measures.

**5- ETL Development:**


* The core of our data integration process is the development of Extract, Transform, Load (ETL) processes. Leveraging SSIS and other ETL tools, we created workflows to extract data, apply transformations, and load it into the star schema.

**6- Data Mart Load:**


* We populated the data mart with cleansed and transformed data, ensuring that it is readily available for analysis.


## Project Workflow:

### Star Schema Design:
Meticulously crafted a star schema that forms the backbone of our data mart. This star schema comprises four dimension tables—Product, Customer, Territory, and Date—and a central fact table housing our key measures and surrogate keys from the dimension tables. This design provides a solid foundation for efficient data analysis and reporting, ensuring that our data mart is well-structured and optimized for our specific analytical needs.


![Sales Data Mart Star Schema](#link)

### SSIS Packages:
I have created six packages to build this data mart 
* dim_Product
* dim_Customer
* dim_Territory
* dim_Date
* Fact_Sales_Full_Load 
* Fact_Sales_Increamental_Load
### Note:
* there is fact table for full load and another for increamental load
