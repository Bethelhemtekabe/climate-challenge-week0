# week0_climate-
1st challenge KAIM
# Climate Challenge Week 0

## Project Overview
This project is part of the Week 0 Climate Challenge, focused on exploring and analyzing climate-related datasets for selected African countries. The main goal is to perform exploratory data analysis (EDA) to understand patterns and trends in climate variables such as rainfall, temperature, and related environmental indicators. Using Python and data science libraries, the project involves data cleaning, visualization, and insight extraction to support better understanding of climate behavior across different regions.

## My Contribution
- Performed data cleaning and visualization on notebooks eda.ethiopia.ipynb,eda.kenya.ipynb,eda.sudan.ipynb,eda.tanzania.ipynb,eda.nigeria.ipynb

## Implementation Summary
- Loaded dataset using pandas
- Cleaned missing values
- Performed exploratory data analysis
- Created visualizations for climate patterns

## Tools Used
- Python
- Pandas
- Matplotlib
- Jupyter Notebook









Regional Climate Analysis & Vulnerability Report (2015–2026)
This project provides a comprehensive analysis of meteorological data for five East and West African countries: Ethiopia, Kenya, Sudan, Tanzania, and Nigeria. The objective is to identify climate trends, analyze precipitation variability, and assess regional vulnerability for the upcoming COP32 summit.

📁 Project Structure
Data/: Contains the raw and cleaned .csv files for each country.

Notebooks/:

ethiopia.eda.ipynb: Individual country analysis.

tanzania.eda.ipynb: Individual country analysis.

combined_comparison.ipynb: Final multi-country integration and COP32 report.

monthly_temp_comparison.png: Visualization of temperature trends across the region.

🛠️ The Pipeline
1. Data Cleaning & Preprocessing

Standardization: Converted date formats to datetime64[ns] to ensure alignment across datasets.

Handling Missing Values: Handled potential gaps in NASA POWER data.

Feature Engineering: Added a Country column to each dataset before concatenation to maintain data lineage.

Normalization: Ensured consistent naming conventions (e.g., T2M, PRECTOTCORR, PS).

2. Exploratory Data Analysis (EDA)

Correlations: Used Seaborn heatmaps to identify strong relationships between Mean Temp (T2M) and Surface Pressure (PS).

Seasonality: Identified the "thermal refuge" characteristics of high-altitude regions.

Distributions: Analyzed temperature and rainfall spreads using histograms and KDE plots.

3. Multi-Country Comparison

Data Integration: Unified five separate datasets into a single master DataFrame.

Resampling: Aggregated daily data into Monthly Means (freq='ME') to identify long-term climate cycles.

Extreme Event Detection: * Quantified Extreme Heat Days (Max Temp >35°C).

Calculated Consecutive Dry Days (CDD) to assess drought risk.

📈 Key Visualizations
Monthly Temperature Trends: A multi-line chart comparing thermal baselines (2015–2026).

Precipitation Boxplots: Side-by-side comparison of rainfall variability and outlier frequency.

Heat Frequency Bars: Annual counts of extreme heat events per country.

🌍 COP32 Vulnerability Ranking
Rank	Country	Primary Risk	Vulnerability
1	Sudan	Thermal Threshold Crossing	Critical
2	Nigeria	Extreme Precipitation Outliers	High
3	Tanzania	Humidity & Heat Stability	Moderate-High
4	Kenya	Seasonal Onset Variance	Moderate
5	Ethiopia	Highland Thermal Stability	Strategic Baseline