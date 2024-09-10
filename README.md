# Amazon Laptop Data Engineering Project

## Overview

In this project, I demonstrate a complete data engineering pipeline, focusing on the extraction, transformation, and loading (ETL) of laptop data from Amazon. Using web scraping, I collect product details, clean and transform the data, store it in a PostgreSQL database, and then perform data analysis to gain insights into laptop pricing and ratings by brand.

## Features

- **Web Scraping**: I crawled laptop data from Amazon, including product name, brand, price, ratings, and specifications like RAM, screen size, and CPU model.
- **Data Cleaning**: I cleaned and preprocessed the scraped data by handling missing values, correcting misplaced entries, and converting data types.
- **Data Transformation**: I transformed the cleaned data into a structured format, preparing it for analysis.
- **PostgreSQL Integration**: I loaded the processed data into a PostgreSQL database for further querying and analysis.
- **Data Analysis**: I analyzed the stored data to calculate average prices and ratings by brand, identified top-rated laptops, and visualized price vs. rating trends.
- **ETL Pipeline**: This project demonstrates a complete ETL pipeline, from data extraction via web scraping to data loading into a PostgreSQL database and analysis using SQL and Python.

## Installation

To run this project, you'll need the following dependencies:

```bash
pip install pandas numpy requests beautifulsoup4 sqlalchemy psycopg2 seaborn matplotlib
```

Additionally, ensure you have PostgreSQL installed and set up on your machine.

## Usage

1. **Clone the repository**:

```bash
git clone https://github.com/qdinh18/amazon-laptop-data-engineering.git
```

2. **Set up the PostgreSQL database**:

   - Create a PostgreSQL database named `postgres` (or customize the database name in the code).
   - Update the connection parameters (host, port, username, password) in the notebook to match your PostgreSQL setup.

3. **Run the Jupyter Notebook**:

   The notebook will:
   - Scrape laptop data from Amazon's product pages.
   - Clean and transform the data.
   - Store the data in the PostgreSQL database.
   - Perform SQL-based analysis on the data.
   - Visualize the relationships between laptop prices and ratings by brand.

## Project Structure

- `Notebook.ipynb`: Contains the complete ETL pipeline, from web scraping to PostgreSQL database storage, analysis, and visualization.

## Data Pipeline

1. **Extract**: I scraped laptop data from Amazon using `requests` and `BeautifulSoup`.
2. **Transform**: I cleaned and processed the data using `pandas` and `numpy`, ensuring that the data was correctly formatted and free of inconsistencies.
3. **Load**: I loaded the cleaned data into a PostgreSQL database using `SQLAlchemy`.
4. **Analyze**: I executed SQL queries to analyze the data and used Python libraries like `seaborn` and `matplotlib` to visualize insights.

## Analysis Highlights

- I identified the laptop brands with the highest average ratings and evaluated laptops under $1000 based on their ratings.
- I visualized the relationship between price and rating by brand through scatter plots.

## Conclusion

This project showcases the full lifecycle of a data engineering task, including web scraping, data cleaning, transformation, and loading into a database. The final analysis provides insights into the relationship between laptop prices and their ratings, helping to identify the best value laptops in the market.
