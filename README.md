# Optimizing-Inventory-Problem-using-SQL

This SQL-based inventory analytics project aims to assist a retail business in identifying stock inefficiencies, enhancing replenishment decisions, and monitoring inventory performance across various stores and products.

**Project Objective**

The project analyzes sales and inventory data to identify several key areas:

* Stockouts and low-inventory products
* Fast-moving and slow-moving products
* Inventory turnover
* Forecast errors
* Seasonal demand patterns
* Products requiring stock increases or reductions

**Database Design**

The raw data is organized into a normalized schema comprising three main tables:

* product_master: Contains product and seasonality information.
* store_master: Stores store and region information.
* sales: This table holds inventory, sales, forecast, pricing, and promotion data.

**Key SQL Analysis**

The project includes various SQL queries to perform the following analyses:

* Current stock level analysis
* Reorder point calculation
* Detection of low-inventory products
* Inventory turnover calculation
* Average inventory levels
* Identification of low-inventory days
* Analysis of forecast errors
* Comparison of fast-moving and slow-moving products
* Recommendations for stock adjustments
* Analysis of supplier and competitor prices
* Identification of seasonal sales trends
* Detection of inventory jumps

Reorder Point
Reorder points are estimated based on recent demand data.
Reorder Point = 7-Day Average Units Sold multiplied by 3 is used to identify products that may need restocking.

Stock Recommendations
Products are categorized into three groups:
* Increase: Low inventory and high turnover
* Reduce: High inventory and low turnover
* Balanced: Inventory within a reasonable range

Performance Optimization
SQL performance was enhanced by adding indexes to frequently used columns such as store_id, product_id, and sales_date.

**Key Insights**
The analysis revealed areas of overstocking, inventory lags, forecast inaccuracies, and potential replenishment issues. These insights provided data-driven recommendations for improved inventory management.

**Technologies**
* SQL
* Case
* Window Functions
* Joins
* Aggregations
* Indexing
* Data Normalization
