LondonBikeTrends

Overview

LondonBikeTrends is a data analysis project that examines bike ride patterns in London between December 22, 2015, and January 29, 2016. The project leverages a dataset of bike rides to explore how weather conditions—such as temperature, wind speed, and weather type—affect ride frequency. Key visualizations include a 14-day moving average of rides and a heatmap illustrating the relationship between temperature, wind speed, and ride counts.

Dataset

The dataset (london_merged.csv) contains hourly bike ride data with the following features:





time: Timestamp of the record



count: Number of bike rides



temp_real_C: Actual temperature in Celsius



temp_feels_like_C: Perceived temperature in Celsius



humidity_percent: Humidity as a percentage



wind_speed_kph: Wind speed in kilometers per hour



weather: Weather condition (e.g., Clear, Rain, Snowfall)



is_holiday: Binary indicator for holidays



is_weekend: Binary indicator for weekends



season: Season of the year (spring, summer, autumn, winter)

Analysis

The analysis is performed in a Jupyter Notebook (london_bike_rides.ipynb) using Python. Key steps include:





Data Preprocessing:





Renaming columns for clarity



Converting humidity to a percentage (0-1 scale)



Mapping numerical codes for weather and season to human-readable labels



Visualization:





A line plot showing the 14-day moving average of bike rides over time



A heatmap displaying bike ride counts across temperature and wind speed bins



A bar chart summarizing ride counts by weather condition



Output:





Processed data saved as london_bikes_final.xlsx

Key Insights





Bike ride frequency fluctuates with weather conditions, with notable dips during adverse weather like rain or snowfall.



The 14-day moving average highlights seasonal trends, with a significant drop around late 2015/early 2016, possibly due to weather or holidays.



The heatmap reveals that rides peak at moderate temperatures (around 7-12°C) and lower wind speeds (0-10 kph).

Requirements

To run the analysis, ensure you have the following Python packages installed:





numpy



pandas



matplotlib



seaborn

Install them using:

pip install numpy pandas matplotlib seaborn

Usage





Clone the repository:

git clone https://github.com/your-username/LondonBikeTrends.git



Navigate to the project directory:

cd LondonBikeTrends



Open the Jupyter Notebook:

jupyter notebook london_bike_rides.ipynb



Run the cells to preprocess the data, generate visualizations, and explore the results.

Files





london_bike_rides.ipynb: Jupyter Notebook containing the analysis code



london_merged.csv: Original dataset (ensure this file is placed in the correct directory as specified in the notebook)



london_bikes_final.xlsx: Processed dataset exported as an Excel file



README.md: Project documentation

Visualization

The main visualization includes:





Moving Average Plot: Tracks the 14-day moving average of bike rides over the analysis period.



Heatmap: Shows bike ride counts as a function of temperature and wind speed.



Weather Bar Chart: Displays total rides by weather condition (e.g., Broken clouds: 14,927 rides, Rain: 1,801 rides).

License

This project is licensed under the MIT License. See the LICENSE file for details.

Author

Created by Atharva Aswale.

Acknowledgments





Data sourced from publicly available London bike ride records.



Built using Python, pandas, matplotlib, and seaborn.
