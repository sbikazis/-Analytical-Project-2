Data Cleaning • Visualization •  Insights Extraction

By: Zakaria Sbika


Project Overview

This project presents a full analysis of a weather dataset for 10 days of January, including temperature, humidity, weather conditions, and wind speed.

The goal of this project is to demonstrate practical data analysis skills using Python, Pandas, Matplotlib, and to extract meaningful insights from real-world weather data.




 Dataset Description

The dataset used in this project contains the following columns:

Column Name	Description

Date	Day of the month (converted to datetime)
Temperature	Daily temperature in °C
Humidity	Humidity level (%)
WindSpeed	Wind speed in km/h
Condition	Weather condition (Sunny, Rainy, Cloudy, etc.)


🛠 Steps Completed in the Project

✔ 1. Importing and Loading the Dataset

df = pd.read_csv("wether_data.csv")

✔ 2. Initial Exploration

Displayed the first 5 rows

Checked missing values

Checked for duplicated rows


✔ 3. Data Cleaning

Converted Date column into datetime

Extracted Month and Day

Created a new feature Temp_Category (Cold / Warm / Hot)


def temkind(tem):
    if tem < 12:
        return "Cold"
    elif tem >= 12 and tem <= 17:
        return "Warm"
    else:
        return "Hot"




 Analysis Results

🌡 Average Temperature

14.5°C

☀ Most Frequent Weather Condition

Sunny (50% of the days)

💧 Highest Humidity

75%

Recorded on January 8th


🌬 Lowest Wind Speed

16 km/h

Recorded on January 10th



 Visualizations

1️⃣ Temperature Variation Over Days

A line chart showing how temperature increased, dropped, and increased again during the 10 days.

2️⃣ Average Temperature per Weather Condition

A bar chart comparing temperatures across (Sunny, Cloudy, Rainy…).

3️⃣ Condition Distribution

A pie chart showing the percentage of each weather condition in January.



 Key Insights

Temperature rose on days 1 and 2, then dropped on 3 and 4.

A strong rise happened on day 6, reaching 18°C.

It dropped again by day 8 (~11°C).

It increased sharply on the last two days, reaching 19°C.

Sunny days dominated the dataset with 50% occurrence.

Day 8 had extremely high humidity.

Day 4 had the weakest wind speed.



 Technologies Used

Python

Pandas

Matplotlib

Jupyter Notebook

👤 Author

Zakaria Sbika
Data Analyst (Beginner Level) — Building portfolio projects step by step.
