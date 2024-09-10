World Life Expectancy Project
This project provides an in-depth analysis of global life expectancy trends over time, focusing on the impact of economic factors like GDP, health metrics such as BMI, and country classifications (developed vs. developing). The data was cleaned, and several SQL queries were run to extract meaningful insights.

Project Overview
The purpose of this project is to explore life expectancy data from various countries across multiple years. The dataset has been cleaned to remove duplicates, handle missing values, and ensure data integrity. Several SQL queries were executed to gather insights and analyze trends in the data.

Files in this Repository
world_life_expectancy_cleaned_up.xlsx: The cleaned dataset containing information on life expectancy, GDP, and other health and socio-economic indicators.

queries.sql: SQL queries used to clean the dataset and perform exploratory data analysis (EDA). These queries include duplicate removal, filling missing data, and deriving insights on life expectancy trends.

README.md: This file, providing a description of the project and its contents.

Data Cleaning Steps
The following SQL queries were used to clean and prepare the data for analysis:

Identifying and removing duplicate records: Ensured that no country-year combination was counted more than once.
Handling missing status information: Updated missing country statuses (developed vs. developing) based on existing data.
Filling missing life expectancy data: Estimated missing life expectancy values using data from surrounding years to improve data continuity.
Exploratory Data Analysis (EDA)
Key insights were gathered using SQL queries that addressed the following:

Life expectancy changes over time by country.
Average life expectancy by year, showing global trends.
Comparing GDP and life expectancy, highlighting the relationship between wealth and health outcomes.
Comparing life expectancy between developed and developing countries, illustrating differences based on country status.
Life expectancy vs. BMI, showing the health impact of BMI on life expectancy.
Cumulative adult mortality for selected countries, providing a long-term view of mortality trends.
Key SQL Queries
Life Expectancy by Year: SELECT Year, ROUND(AVG(Life expectancy),2)
Provides yearly average life expectancy values globally.

Life Expectancy vs. GDP: SELECT Country, ROUND (AVG(Life expectancy),1) AS Life_exp, ROUND(AVG(GDP),1) AS GDP
Shows the relationship between a country's average life expectancy and GDP.

Developed vs. Developing Countries: SELECT Status, ROUND(AVG(Life expectancy),1)
Compares life expectancy between developed and developing countries.
