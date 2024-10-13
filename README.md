# Layoffs Data Analysis

## Project Overview

This project focuses on analyzing layoffs data using SQL, divided into two main sections: 

1. **Data Cleaning**: Cleaning and standardizing the data to ensure accuracy and consistency.
2. **Exploratory Data Analysis (EDA)**: Performing data analysis to uncover insights on layoffs by company, industry, country, and trends over time.

The dataset contains information about layoffs from various companies, including details such as company name, location, industry, total layoffs, percentage laid off, and funding raised.

## Dataset

The dataset `layoffs_data.csv` includes the following columns:

- `company`: Name of the company
- `location`: Location of the company
- `industry`: Industry type
- `total_laid_off`: Total number of employees laid off
- `percentage_laid_off`: Percentage of employees laid off
- `date`: Date of the layoffs
- `stage`: Company growth stage
- `country`: Country of the company
- `funds_raised_millions`: Total funds raised by the company (in millions)

## Project Structure

The project is divided into two SQL files:

- **Data_Cleaning.sql**: This file contains all SQL queries related to cleaning and standardizing the data, including:
  - Removing duplicates
  - Handling null values and blank fields
  - Standardizing company names, industry types, and date formats
  - Deleting unnecessary rows and columns
  - Updating data inconsistencies using joins and conditional updates

- **EDA.sql**: This file contains SQL queries related to the exploratory data analysis of the cleaned dataset, including:
  - Summing up total layoffs by company, industry, and country
  - Calculating rolling totals of layoffs over time
  - Analyzing layoffs trends by year and company growth stage
  - Ranking companies by the number of layoffs in a given year

## Queries Breakdown

### Data Cleaning
- **Removing Duplicates**: Duplicate entries based on key columns are identified and removed.
- **Standardizing Data**: Standardizing company names, industry types, and trimming extra spaces and characters for consistency.
- **Handling Missing Data**: Managing missing values in the `industry` column, and removing rows where both `total_laid_off` and `percentage_laid_off` are null.
- **Date Standardization**: Converting date formats to a standard `DATE` type for accurate time-based analysis.

### Exploratory Data Analysis (EDA)
- **Layoff Trends by Company**: Identifying companies with the highest number of layoffs.
- **Industry and Country Analysis**: Summing layoffs by industry and country to identify key areas affected by layoffs.
- **Date and Yearly Trends**: Analyzing layoffs by year and identifying trends over time.
- **Company Rankings**: Ranking companies by layoffs each year using SQL window functions.
- **Rolling Total of Layoffs**: Calculating the cumulative total of layoffs month by month.


## Conclusion

This project demonstrates the use of SQL for data cleaning and analysis, with a focus on understanding trends in layoffs across various companies and industries. By leveraging SQL's powerful querying capabilities, we were able to extract meaningful insights and trends from the dataset.



