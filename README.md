# Data Warehouse Final Project

## Overview

This project involves building a Data Warehouse solution using the OLTP e-commerce dataset from Kaggle as the data source. The ETL process is implemented using SQL Server Integration Services (SSIS), and the data is modeled into a star schema to facilitate efficient analysis and reporting.

## Dataset

- **Source**: [OLTP e-commerce dataset on Kaggle](https://www.kaggle.com/datasets/sharangkulkarni/oltp-ecommerce-data)
- **Description**: The dataset contains transactional data from an e-commerce platform, including information on customers, orders, products, payments, and reviews.

## ETL Process

- **Tool**: SQL Server Integration Services (SSIS)
- **Steps**:
  1. **Extraction**: Data is extracted from the source CSV files provided in the Kaggle dataset.
  2. **Transformation**: Data is cleaned and transformed to match the structure of the target data warehouse schema.
  3. **Loading**: Transformed data is loaded into the data warehouse implemented in SQL Server.

## Getting Started

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/AHmEeD-SaBER/DWH_Final_Project.git
   ```

2. **Configure SSIS**:
   - Open the SSIS packages in the `SSIS_Packages` directory using SQL Server Data Tools.
   - Update the connection strings to match your environment.

3. **Run ETL Process**:
   - Execute the SSIS packages in the following order:
     1. `Load_STG`
     2. `Load_Dimensions`
     3. `Load.factTables`

4. **Verify Data**:
   - Query the data warehouse to ensure data has been loaded correctly.

## Author

- **Ahmed Saber** - [GitHub Profile](https://github.com/AHmEeD-SaBER)

## License

