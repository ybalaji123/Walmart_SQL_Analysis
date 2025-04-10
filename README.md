# Walmart Analysis Using SQL(SSMS)

![walmart data](https://github.com/ybalaji123/Walmart_SQL_Analysis/blob/main/walmart_image.jpg)

# Overview
This project aims to explore the Walmart Sales data to understand top performing branches and products, sales trend of of different products, customer behaviour. The aims is to study how sales strategies can be improved and optimized

"In this recruiting competition, job-seekers are provided with historical sales data for 45 Walmart stores located in different regions. Each store contains many departments, and participants must project the sales for each department in each store. To add to the challenge, selected holiday markdown events are included in the dataset. These markdowns are known to affect sales, but it is challenging to predict which departments are affected and the extent of the impact

# Purposes Of The Project
The major aim of thie project is to gain insight into the sales data of Walmart to understand the different factors that affect sales of the different branches.

# Installation of SSMS(SQL Server management Studio)
Click the following link to download and install SQL Server Management Studio (SSMS).
- **Youtube** [Click link](https://www.youtube.com/watch?v=iaUXjTL_F9U)

# Dataset
The data for this project is sourced from the Kaggle dataset

- **Dataset Link:** [Dataset](https://github.com/ybalaji123/Walmart_SQL_Analysis/blob/main/WalmartSalesData.csv.csv)

# Schema
```sql
-- Create database
create database Walmart

-- Create table
CREATE TABLE walmart(
	invoice_id VARCHAR(30) NOT NULL PRIMARY KEY,
    branch VARCHAR(5) NOT NULL,
    city VARCHAR(30) NOT NULL,
    customer_type VARCHAR(30) NOT NULL,
    gender VARCHAR(30) NOT NULL,
    product_line VARCHAR(100) NOT NULL,
    unit_price DECIMAL(10,2) NOT NULL,
    quantity INT NOT NULL,
    tax_pct FLOAT(6,4) NOT NULL,
    total DECIMAL(12, 4) NOT NULL,
    date DATETIME NOT NULL,
    time TIME NOT NULL,
    payment VARCHAR(15) NOT NULL,
    cogs DECIMAL(10,2) NOT NULL,
    gross_margin_pct FLOAT(11,9),
    gross_income DECIMAL(12, 4),
    rating FLOAT(2, 1)
);
```
