# San Francisco Bay Area Real Estate Analysis

## Overview
This project involves a comprehensive analysis of the real estate market in the San Francisco Bay Area. By collecting and analyzing data on property prices, rental rates, and market trends, the project aims to provide insights into market dynamics and identify key factors influencing property values. The housing and rental prices in this region have been accelerating at shocking rates. From 2010 to 2017, the median price of a single-family home in San Francisco increased from approximately $775,000 to $1.5 million.

## Objectives
- Collect information on more than 600 distinct properties from the Redfin Real Estate website
- Clean, prepare, organize, and handle missing data, outliers, and incorrect records
- Prepare a statistical report to analyze current market trends in real estate
- Propose and address several research questions using visualization techniques

## Data Collection
We used two main methods for data collection:
1. Selenium Automation:
  - Bot opens the website and locates required attributes
  - Extracts the required attributes
  - Converts the data into a suitable format
  - Repeats the process for all pages

2. HTML Parser:
  - Uses custom headers to avoid HTML content backlog
  - Identifies HTML tags for required attributes
  - Extracts tag content and repeats the process for all pages

## Data Cleaning
- Initially extracted over 1200 data points from six different counties
- After cleaning, the dataset was reduced to approximately 430 entries
- Cleaning process involved: Removing null values, Splitting alphanumeric data into categorical and quantitative columns

## Exploratory Data Analysis (EDA)
Our EDA addressed the following questions:
- Cities with the highest and lowest average price per square foot per county
- Distribution of houses based on the number of bathrooms and bedrooms
- Sales price distribution
- Impact of walk score and bike score on house prices
- Effect of school ratings on house prices
- Distribution of property types based on counties
- Correlation between different features of houses in the dataset

## Usage
- Load the real estate dataset.
- Run the scripts to perform data cleaning, analysis, and modeling.
- Visualize the results to understand market trends and price predictions.

## Key Findings
- Santa Clara County has the highest per square foot price, followed closely by San Mateo County
- Contra Costa County has the lowest per square foot price, less than half of Santa Clara or San Mateo counties
- Houses with 3 bedrooms and 2 bathrooms are the most common listings
- The sales price distribution is right-skewed with some extreme higher values
- There's a very weak positive correlation between walk score and house price
- School ratings have a significant impact on house prices, with "Excellent" rated areas commanding higher prices

## Predictive Analysis
We used several machine learning techniques for price prediction:
- Linear Regression
- Random Forest Regressor

We analyzed these models using K-fold Cross-Validation and compared their performance.

## Features
- Data scraping and cleaning from multiple real estate sources
- Exploratory data analysis to identify trends and correlations
- Predictive modeling to estimate property prices and rental rates
- Geospatial analysis to visualize property distributions and hotspots

## Technologies Used
- **Programming Languages**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, BeautifulSoup, Selenium, Matplotlib, Seaborn, GeoPandas
- **Tools**: Jupyter Notebook

## Future Work
- Incorporate more recent data to track ongoing trends
- Expand the analysis to include more counties or cities
- Develop a user-friendly interface for real-time price predictions

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.
