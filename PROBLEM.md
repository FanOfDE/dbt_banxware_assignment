# Data Engineering Home Assignment

## Objective

The purpose of this assignment is to evaluate your ability to work with data pipelines, perform data transformations, and optimize a data warehouse setup. You have been provided with a sample dataset and asked to perform a series of tasks to demonstrate your understanding of data engineering concepts.

## Problem

Our company has recently launched a new product and we are looking to analyze the sales data to understand its performance. Our sales team came up with a few questions that they would like to answer using the data:

- What are the top 5 products by total sales amount in the year 2023?
- What are the names of the top 5 customers by total sales amount in the year 2023?
- What is the average order value for each month in the year 2023?

### Setting Up Your Environment:

Create a new Snowflake account (It’s free for 30 days) and set up a database named home_assignment.
Install dbt (data build tool) and configure it to connect to your Snowflake database.

### Data Ingestion:

You have been provided with 2 csv files under the `data` folder:

- sales.csv
- customers.csv

Both contain fictional data and are used for this assignment.

Using any data ingestion tool of your choice, create a process to ingest the `sales.csv` into your Snowflake database into a table named `raw_sales_data`.

### Data Transformation:

Use dbt to create a model that transforms `raw_sales_data` into a more structured format for analysis. Name this table `transformed_sales_data`.

Include the following transformations:

Extract year, month, and day from the `order_date` field.

Calculate the total sales amount for each order.

## Submission

- Document each step of your process, explaining your setup, transformations, and any decisions made during the assignment in a file named `DECISIONS.md`.
- Publish your project to a public GitHub repository and share the link with us.
- Include the SQL query file for the analysis in a folder named `queries`.

## Evaluation Criteria

- Correctness: Does your solution correctly load, transform, and query the data?
- Efficiency: Are your SQL queries and data transformations optimized?
- Clarity: Is your code well-documented and easy to understand?
- Completion: Did you complete all parts of the assignment and provide all required files?
