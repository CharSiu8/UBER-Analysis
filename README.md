# Uber Data Analysis: NYC Pickup Demand

## 📌 Context
Uber Technologies, Inc. is a global leader in the ridesharing market, operating in approximately 72 countries and 10,500 cities. The ridesharing industry is highly volatile, with demand fluctuating based on time, location, weather conditions, and local events. To remain successful, it is critical for Uber to detect these patterns and adapt its operations accordingly.

## 🎯 Project Objective
The primary goal of this project is to extract actionable insights from demand patterns to help the business understand its demand profile and drive better outcomes.

### Key Questions Addressed:
1. What variables influence ride pickups in NYC?
2. Which factor has the most significant impact on demand?
3. What are the management recommendations for capitalizing on these fluctuations?

## 📊 Dataset Overview
The dataset covers hourly ride and weather information for New York City starting from January 1st, 2015.

| Feature | Description |
| :--- | :--- |
| `pickup_dt` | Date and time of the pickup |
| `borough` | The NYC borough where the ride originated |
| `pickups` | Number of pickups during that 1-hour period |
| `spd` / `vsb` | Wind speed (mph) and Visibility (miles) |
| `temp` / `dewp` | Temperature and Dew point (Fahrenheit) |
| `pcp01` / `06` / `24` | Liquid precipitation (1-hour, 6-hour, and 24-hour) |
| `sd` | Snow depth in inches |
| `hday` | Holiday indicator (Y/N) |

## 🛠️ Methodology
The analysis follows a standard data science workflow:
* **Exploratory Data Analysis (EDA):** Univariate and bivariate analysis of weather and temporal features.
* **Feature Engineering:** Using the `datetime` library to extract granular time-based features.
* **Visualization:** Utilizing `Seaborn` and `Matplotlib` to identify trends across different NYC boroughs