# RUSH Sales Data Analysis

## Overview

This project analyzes U.S. sales data for RUSH, a sportswear and footwear brand. The goal of the analysis is to identify sales trends, understand product and retailer performance, and uncover opportunities for growth.

The analysis was completed using Python and Pandas in a Google Colab notebook.

## Business Objective

The VP of U.S. Sales wants to better understand the company's sales performance across products, retailers, locations, and sales methods. This analysis addresses several key business questions and explores additional trends that can help inform sales and growth decisions.

## Data

The raw data was provided as three separate tables:

* **TABLE_PRODUCTS** — Contains product IDs and product names.
* **TABLE_RETAILER** — Contains retailer IDs, retailer names, regions, states, and cities.
* **TABLE_SALES** — Contains order information, invoice dates, products, prices, units sold, operating margins, and sales methods.

The three tables were merged using `PRODUCT_ID` and `RETAILER_ID`.

## Data Preparation

The dataset was examined and cleaned before analysis. Key preparation steps included:

* Checking the shape and structure of each table
* Merging the three tables together
* Identifying missing values
* Filling missing product prices using the median price for the corresponding product ID
* Replacing an invalid retailer ID and missing retailer/location information with `"Unknown"`
* Converting different columns to the correct data types
* Identifying and correcting outlier values
* Checking for duplicate rows
* Investigating duplicate order IDs
* Checking categorical values for inconsistencies in spelling/capitalization
* Calculating sales by multiplying two other columns together

## Business Questions

The analysis answers the following questions:

1. What product category had the highest sales in 2021?
2. What state had the highest sales of women's products in 2021?
3. What state had the highest sales of men's products in 2021?
4. What retailer purchased the most units in 2021 and 2020?

## Tools Used

* Python
* Pandas
* Google Colab
* GitHub

## Files

* `RUSH_Sales_Data_Analysis.ipynb` — Google Colab/Jupyter Notebook containing the data preparation, exploratory data analysis, business questions, and findings.
* RUSH Data Dictionary.pdf - Data dictionary for better understanding of the data. 
* `TABLE_PRODUCTS_885.csv` — Product data.
* `TABLE_RETAILER_885.csv` — Retailer and location data.
* `TABLE_SALES_885.csv` — Sales transaction data.

## Conclusion

The analysis shows substantial growth in RUSH sales from 2020 to 2021, with Men's Street Footwear emerging as a leading product category and Foot Locker as a major retailer. The results also highlight geographic and sales-channel differences that may provide opportunities for targeted growth strategies.

Further analysis of year-over-year retailer growth, product profitability, and seasonal trends could help RUSH identify where to focus future sales and marketing efforts.
