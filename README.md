# prophet-challenge
Prophet Challenge

# MercadoLibre Search Traffic and Stock Price Analysis

This project analyzes the relationship between Google search traffic data and the stock price of MercadoLibre. By leveraging time series analysis and predictive modeling, we aim to uncover patterns in search behavior and their potential connection to financial events, including stock price fluctuations. The project includes forecasting future search trends using Prophet.

## Project Overview

The project is divided into four main steps:
1. **Find Unusual Patterns in Hourly Google Search Traffic**
2. **Mine the Search Traffic Data for Seasonality**
3. **Relate the Search Traffic to Stock Price Patterns**
4. **Create a Time Series Model with Prophet**

## Instructions

### Step 1: Find Unusual Patterns in Hourly Google Search Traffic
The goal of this step is to determine if Google search traffic patterns are linked to any significant corporate financial events. This includes visualizing the data for unusual patterns and comparing the search trends during the release of MercadoLibre's quarterly financial results in May 2020.

#### Key Tasks:
- Read the search data into a DataFrame and filter to May 2020.
- Visualize any unusual patterns.
- Calculate total search traffic for May 2020.
- Compare the total search traffic to the monthly median across all months.
- Analyze if search traffic increased during the release of financial results.

### Step 2: Mine the Search Traffic Data for Seasonality
Marketing is interested in determining if there are seasonal patterns in the search traffic data. By tracking these patterns, marketing efforts can be optimized.

#### Key Tasks:
- Group the search data by hour of the day, day of the week, and week of the year.
- Visualize the traffic patterns.
- Identify any time-based trends and their potential impact on marketing.

### Step 3: Relate the Search Traffic to Stock Price Patterns
The finance team has asked if a relationship exists between the search data and MercadoLibre's stock price. This step involves merging the search traffic data with stock price data and investigating any potential relationships.

#### Key Tasks:
- Read and plot the stock price data.
- Concatenate the stock price and search traffic data.
- Slice the data to the first half of 2020 and investigate any common trends.
- Create new columns for "Lagged Search Trends", "Stock Volatility", and "Hourly Stock Return".
- Explore correlations between search trends and stock price metrics.

### Step 4: Create a Time Series Model with Prophet
In the final step, we use Facebook's Prophet library to build a time series forecasting model for the search traffic data.

#### Key Tasks:
- Set up the Google search data for a Prophet model.
- Estimate the model and plot the forecast.
- Analyze the time series components to answer questions about daily, weekly, and yearly trends.
  - What time of day exhibits the greatest popularity?
  - Which day of the week gets the most traffic?
  - What is the lowest point of search traffic in the calendar year?

## Dependencies
- `pandas`
- `Prophet`
- `matplotlib`

## Files
- **forecasting_net_prophet.ipynb**: The Jupyter Notebook containing the full analysis and code implementation.
