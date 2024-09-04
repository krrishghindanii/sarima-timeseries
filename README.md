# Air Quality Forecasting for Shanghai

This project analyzes and forecasts air quality components in Shanghai using historical data and SARIMA (Seasonal AutoRegressive Integrated Moving Average) models.

### Project Overview

The script processes air quality data for Shanghai, visualizes historical trends, and generates forecasts for various air quality components using SARIMA models. It focuses on the following air quality indicators:

- AQI (Air Quality Index)
- CO (Carbon Monoxide)
- NO (Nitric Oxide)
- NO2 (Nitrogen Dioxide)
- O3 (Ozone)
- SO2 (Sulfur Dioxide)
- PM2.5 (Fine Particulate Matter)
- PM10 (Respirable Particulate Matter)
- NH3 (Ammonia)

### Features

1. Data preprocessing:
   - Loads data from 'Shanghai.csv'
   - Filters data for the last 90 days
   - Resamples data to hourly intervals

2. Visualization:
   - Plots historical trends for each air quality component

3. SARIMA Modeling:
   - Fits a SARIMA model to each air quality component
   - Generates 90-day forecasts
   - Visualizes forecasts with confidence intervals

4. Analysis Output:
   - Displays model summaries
   - Prints forecast values

### Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- statsmodels

### Usage

1. Ensure 'Shanghai.csv' is in the same directory as the script
2. Run the script:
   ```
   python air_quality_forecast.py
   ```

3. The script will generate plots and print analysis results for each air quality component

### Data Source

The data is expected to be in a CSV file named 'Shanghai.csv' with a 'dt' column for timestamps and separate columns for each air quality component.
