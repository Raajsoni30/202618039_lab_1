DS605: Fundamentals of Machine Learning

Lab Assignment 1 - Data Scraping and Preprocessing using Python and Scrapy

Name:Raaj Soni
Student ID: 202618039

Project Overview

This project collects book information from the Books to Scrape website using Python and Scrapy.
The scraped data is then cleaned, transformed, analyzed, and visualized using Python.

The project covers the complete process from web scraping to data preprocessing and analysis.

Dataset

The project scrapes at least 100 books from five catalog pages.

The following information is collected:

* Title
* Category
* Price
* Rating
* Availability
* Product description
* UPC
* Number of reviews
* Product URL

Task 1 - Data Scraping

A Scrapy spider is used to:

* Follow catalog pagination.
* Visit individual book pages.
* Extract the required book information.
* Save the raw scraped data as a CSV file.
* Check the total number of records.
* Check missing values.
* Check duplicate UPC values.

Task 2 - Data Preprocessing

The raw data is cleaned and prepared for analysis.

The preprocessing includes:

* Removing extra spaces from text fields.
* Removing duplicate books using UPC.
* Handling missing descriptions.
* Converting prices into numeric values.
* Converting ratings into numeric values.
* Extracting the available stock count.

The following features are also created:

* `description_word_count`
* `price_band`
* `value_score`
* `recommended`

## Task 3 - Visualization and Analysis

Several visualizations are created to understand the dataset:

* Price distribution
* Rating distribution
* Average price by category
* Price versus rating
* Book category counts
* Word cloud using book descriptions

Summary statistics are also used to examine prices, ratings, categories, and stock availability.

## Task 4 - Insights and Interpretation

The analysis focuses on:

* The most represented book categories.
* Categories with higher average prices.
* The relationship between price and rating.
* Highly rated books.
* Books with better value scores.
* Stock availability patterns.

The analysis also discusses the limitations of using data collected from only five catalog pages.

## Project Files

```text
DS605-Lab1/
│
├── README.md
├── books.csv
├── books_cleaned.csv
│
├── Scrapy Project/
│   ├── scrapy.cfg
│   └── book_pipeline/
│
├── pandas_1.ipynb
│
├── category_counts.png
├── plots_overview.png
├── wordcloud.png
└── other generated files
```

Technologies Used

* Python
* Scrapy
* Pandas
* NumPy
* Matplotlib
* Seaborn
* WordCloud
* Jupyter Notebook

Conclusion

This project demonstrates a complete data-processing workflow using Python and Scrapy. 
The scraped book data is collected, cleaned, transformed, visualized, and analyzed to identify useful patterns in book prices,
ratings, categories, stock availability, and value.
