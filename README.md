# EDA and Feature Engineering of Google Play Store Dataset

## Table of Contents
1. [Problem Statement](#problem-statement)
2. [Data Collection](#data-collection)
3. [Steps to Follow](#steps-to-follow)
4. [Import Required Libraries](#import-required-libraries)
5. [Data Loading](#data-loading)
6. [Data Cleaning](#data-cleaning)
7. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
8. [Feature Engineering](#feature-engineering)
9. [Visualizations](#visualizations)
10. [Insights](#insights)
11. [Conclusion](#conclusion)

## Problem Statement

Today, 1.85 million different apps are available for users to download. Android users have even more from which to choose, with 2.56 million available through the Google Play Store. These apps have come to play a huge role in the way we live our lives today. Our objective is to find the most popular category, the app with the largest number of installs, the app with the largest size, etc.

## Data Collection

The dataset consists of 20 columns and 10841 rows.

## Steps to Follow

1. Data Cleaning
2. Exploratory Data Analysis
3. Feature Engineering

## Data Cleaning

The dataset was loaded and the initial summary was obtained to understand the structure and the presence of missing values. Several data cleaning steps were undertaken:

- Handling missing values in various columns.
- Converting the 'Reviews' column to integer type.
- Converting 'Size' column to a numeric format, and handling variations such as 'M', 'k', and 'Varies with device'.
- Cleaning 'Installs' and 'Price' columns by removing unnecessary characters and converting them to appropriate numeric types.
- Converting the 'Last Updated' column to datetime format.
- Handling duplicates to ensure each app is unique in the dataset.

## Exploratory Data Analysis (EDA)

### Univariate Analysis

- **Numerical Features:** We performed univariate analysis on numerical features such as 'Rating', 'Reviews', 'Size', 'Installs', 'Price', and observed their distributions.
- **Categorical Features:** Univariate analysis was also performed on categorical features like 'Type' and 'Content Rating' to understand the count distributions.

### Popular App Categories

- Identified the most popular app category by visualizing the distribution of apps across different categories.
- Generated insights about the top 10 app categories based on the number of apps available in each category.

### Most Installed Apps

- Identified the top 5 most installed apps within each popular category and saved this information for further analysis.

### Apps with 5 Ratings

- Found the total number of apps that have a perfect 5-star rating.

### Categories with Largest Installations

- Analyzed which categories have the largest number of installations and visualized this information to highlight the most popular categories in terms of user installs.

## Feature Engineering

- Extracted additional date-related features such as 'Day', 'Month', and 'Year' from the 'Last Updated' column to enable further analysis based on time.

## Visualizations

- Created various plots to visualize the distribution of numerical and categorical features.
- Visualized the most popular app categories using pie charts and bar plots.
- Highlighted the categories with the largest number of installations through bar plots.

## Insights

1. The Family category has the most number of apps with 18% of apps belonging to it, followed by Games category which has 11% of the apps.
2. The least number of apps belong to the Beauty category with less than 1% of the total apps.
3. There are 271 apps having a 5-star rating.
4. The top 5 most installed apps in each popular category have been identified and saved in a CSV file.
5. The category with the largest number of installations is visualized, showing significant trends in user preferences.

## Conclusion

This project provided insights into the Google Play Store dataset through data cleaning, exploratory data analysis, and feature engineering. The visualizations helped identify popular app categories, highly installed apps, and other significant trends within the dataset. The findings can help app developers and marketers make informed decisions based on user preferences and trends.
