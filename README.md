# Bike Sharing Demand Analysis Project

## Project Overview
This project analyzes bike-sharing demand for BoomBikes, a US bike-sharing provider, to help them understand and optimize their business strategy post-COVID pandemic. The analysis aims to identify factors affecting bike rental demand and provide actionable insights for business growth.

## Business Problem
- BoomBikes has experienced revenue decline during the COVID pandemic
- Need to understand post-pandemic demand factors
- Goal to accelerate revenue recovery and growth
- Requirement to develop a mindful business strategy

## Dataset Description
The dataset contains daily bike rental records including:
- Environmental factors (temperature, humidity, windspeed)
- Date-related features (season, year, month, holiday)
- Rental numbers (casual, registered, total)

### Features Information
- season: Spring, Summer, Fall, Winter
- year: 2018, 2019
- month: 1 to 12
- holiday: Binary (0: No, 1: Yes)
- weekday: 0-6
- workingday: Binary (0: No, 1: Yes)
- weathersit: 
  - Clear
  - Mist + Cloudy
  - Light Rain/Snow
  - Heavy Rain/Snow
- temp: Temperature in Celsius (normalized)
- atemp: "Feels like" temperature
- humidity: Normalized humidity
- windspeed: Normalized wind speed
- casual: Count of casual users
- registered: Count of registered users
- cnt: Total rentals (Target variable)

## Analysis Approach
1. Data Preprocessing
   - Feature engineering
   - Handling categorical variables
   - Data cleaning and normalization

2. Exploratory Data Analysis
   - Temporal patterns analysis
   - Weather impact assessment
   - User behavior analysis
   - Correlation studies

3. Model Development
   - Feature selection
   - Linear regression modeling
   - Model evaluation and validation

## Key Findings
1. Temporal Patterns
   - Peak rentals during Fall season (avg: 5,644 rentals)
   - Strong weekend usage patterns
   - Year-over-year growth rate: 64.73%

2. Weather Impact
   - Clear weather averages 4,877 rentals
   - Temperature shows strong positive correlation (r=0.63)
   - Rain reduces rentals by approximately 50%

3. User Behavior
   - 81.2% are registered users
   - Different patterns for casual vs registered users
   - Holiday impact varies by season

## Business Recommendations
1. Seasonal Strategy
   - Optimize fleet size for peak seasons
   - Implement season-based pricing
   - Develop maintenance schedules for off-peak periods

2. Weather-Based Planning
   - Dynamic pricing based on weather conditions
   - Weather-based marketing campaigns
   - Alternative revenue strategies for adverse weather

3. Customer Segmentation
   - Targeted promotions for casual users
   - Loyalty programs for registered users
   - Special holiday offerings

## Model Performance
- R² Score: 0.7751
- RMSE: 877.38 rentals
- Confidence Level: 95% prediction interval

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Statsmodels

## Project Structure
```
day.csv
bike_sharing_analysis.ipynb
README.md
requirements.txt
```
