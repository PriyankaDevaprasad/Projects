📝 Problem Statement

Literacy rates are a vital measure of a country’s human development, economic growth, and educational outreach. 
In this project, we analyze adult literacy, youth literacy, illiteracy population, GDP, and years of schooling data across countries and years. 
The aim is to uncover patterns, correlations, and disparities in education across the globe.

Data Understanding 🔍

Load each dataset into separate Pandas DataFrames and merge datasets on common columns as follows:

df_literacy → Adult & Youth Literacy Rates

df_illiteracy → Illiterate Population Data

df_gdp_schooling → GDP & Years of Schooling
________________________________________
3️⃣ Data Cleaning 🧹
●	Handle missing values: Drop or impute.
●	Remove duplicates.
●	Standardize country names for merging.
●	Understand the shape and structure of the data
●	Identify any unusual values
●	Rename column names for clarity
●	Filter years between 1990 - 2023 (or last year in the data collected)
________________________________________
4️⃣ ⚙️Feature Engineering 
Creating new columns can help uncover deeper insights from the data. Below are some ideas learners can start with — but are encouraged to experiment and create as many new features which can enhance the analysis.
Feature Name	Purpose
Illiteracy %	Shows the percentage of the population that is illiterate.
Literacy Gender Gap	Highlights the disparity between male and female literacy rates.
GDP per Schooling Year	Helps analyze economic output per year of education.
Education Index	Measures education quality by considering both access (literacy) and duration (schooling).
Youth Literacy Average	Provides a single indicator for overall youth literacy.
Literacy Growth Rate	Measures year-over-year improvement in literacy.
________________________________________
📊 Exploratory Data Analysis (EDA) 
Learners should perform both univariate and bivariate analysis to understand the data distribution and relationships.
Guidelines:
●	Use visualization libraries like Matplotlib, Seaborn, or Plotly for plots.

●	Univariate Analysis: Explore each variable individually (e.g., histograms, box plots, bar charts for literacy rates, GDP, etc.).

●	Bivariate Analysis: Explore relationships between variables (e.g., scatter plots of GDP vs Literacy Rate, heatmaps of correlations, line plots over time).

●	Look for trends, seasonal patterns, outliers

●	Summarize findings with insights from the plots.
________________________________________
5️⃣ Data Storage in SQL 🗄️
●	Create 3 tables:
○	literacy_rates 
○	illiteracy_population
○	gdp_schooling 
●	Define composite keys: (country, year) for each table.
________________________________________
7️⃣ SQL Queries 🧮
 literacy_rates
1.	Get top 5 countries with highest adult literacy in 2020.

2.	Find countries where female youth literacy < 80%.

3.	Average adult literacy per continent (owid region).

illiteracy_population
     4. Countries with illiteracy % > 20% in 2000.
     5. Trend of illiteracy % for India (2000–2020).
     6. Top 10 countries with largest illiterate population in the last year.
gdp_schooling
    7. Find countries with avg_years_schooling > 7 and gdp_per_capita < 5000.
    8. Rank countries by GDP per schooling for the year 2020.
    9. Find global average schooling years per year.
Join Queries 
   10. List top 10 countries in 2020 with highest GDP per capita but lowest average years of schooling(less than 6).
  11. Show countries where the illiterate population is high despite having more than 10 average years of schooling.
   12. Compare literacy rates and GDP per capita growth for a selected country over the last 20 years. (country of your choice)
  13. Show the difference between youth literacy male and female rates for countries with 
