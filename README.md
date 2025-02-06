# South Carolina Energy Analysis ⚡🌱

## Project Overview 🌍
This project aims to address the challenges faced by an energy company (eSC) operating in South Carolina and parts of North Carolina during the summer months, particularly in July. The primary objective is to mitigate the risk of blackouts caused by increased electricity demand due to rising temperatures. Instead of expanding energy production infrastructure, the project focuses on understanding the drivers of energy consumption and implementing demand-side management strategies to encourage residential customers to adopt energy-saving practices.

---

## Project Scope 🎯

### Objective
The project seeks to:

- Analyze historical energy consumption data to identify key drivers of increased usage 🔍📊
- Develop and implement strategies to encourage energy-saving practices among residential customers 💡🌱
- Engage with local communities to foster a culture of responsible energy use 🤝🏡
- Monitor and evaluate the effectiveness of energy-saving strategies 📈🔧

### Key Components 🛠️

#### 1. Data Analysis and Insight Generation 📊
- Analyze historical energy consumption data 📅
- Understand patterns and trends related to energy consumption 🔎
- Assess the impact of temperature rise on energy demand 🌡️

#### 2. Demand-Side Management Strategies 🔋
- Develop strategies to encourage energy-saving practices ⚡
- Promote the adoption of energy-efficient technologies 💡🔌
- Initiate educational campaigns to raise awareness about energy conservation 📚💬

#### 3. Community Engagement and Behavioral Change 🏘️
- Engage with local communities to foster responsible energy use 👥🌍
- Implement incentive programs to encourage energy-efficient behaviors 💰
- Monitor the effectiveness of community engagement initiatives 📊

#### 4. Monitoring and Evaluation 📏
- Establish metrics to measure the success of energy-saving strategies 🧮
- Conduct regular assessments to ensure project goals are being met 📅

---

## Project Deliverables 📑

### 1. Data Collection and Cleaning 🧹
- Gather historical data on electricity consumption, weather patterns, and demographic variables 🌡️📈
- Clean the dataset to ensure reliability in subsequent analysis 🧼

### 2. Energy Consumption Analysis 📉
- Use linear regression models to identify key factors impacting energy consumption 🔄
- Analyze these factors to understand their contribution to overall energy demand 📊

### 3. Predictive Modeling for Demand Forecasting 🔮
- Implement advanced predictive models (e.g., Support Vector Machines) to forecast electricity demand ⏳
- Generate actionable insights to inform the energy company's planning and response strategies 💡

### 4. Shiny Apps 🖥️
Develop a Shiny app to visualize energy consumption data, allowing users to:
- Select specific cities within South Carolina to analyze energy usage 🏙️
- View state-wide energy consumption trends 🌍
- Dive into detailed energy usage patterns for individual cities 🔍

---

## Data Description 📚

### 1. Static House Data 🏡
- Contains information on a random sample of single-family houses served by eSC.
- Includes house attributes such as size, stored in 'parquet' format 📦
- Approximately 5,000 houses are represented 🏠

### 2. Energy Usage Data ⚡
- Captures hourly energy usage for each house in the Static House Data ⏱️
- Stored in 'parquet' format, with approximately 5,000 individual datasets ⚙️

### 3. Meta Data 📝
- Provides a human-readable guide to the fields used in the Static House Data and Energy Usage Data 📚
- Likely stored in plain text or CSV format 📄

### 4. Weather Data 🌦️
- Contains hourly weather information for each geographic area or county 🌍
- Stored in CSV format, with approximately 50 weather files 📑

---

## Data Preparation 🔄

- **City Filtering**: Segment cities into "not in census place" and "in census place" categories 🌆
- **Date Conversion**: Convert the date column into a datetime format 📅
- **Data Merging**: Merge Static House Data and Energy Data using building data as a key 🔑
- **County-Level Aggregation**: Aggregate total humidity and temperature data at the county level 🌦️
- **Data Integration**: Integrate county-level data with individual house-level data 🏡
- **Grouping Entire Counties**: Group total humidity and temperature data by county 🏘️

---

## Exploratory Data Analysis (EDA) 🔍

### Visualizations 📊

- **Daily Energy Consumption Trend**: Line chart showing daily energy consumption over time 📉
- **County-wise Total Energy Consumption**: Bar chart comparing total energy consumption across counties 🌍
- **Temperature vs. Energy Consumption**: Scatter plot with a regression line to explore the relationship between temperature and energy consumption 🌡️➡️⚡
- **Humidity vs. Energy Consumption**: Scatter plot to examine the relationship between humidity levels and energy consumption 🌦️➡️⚡
- **Percentage Distribution of Usage Levels by Climate Zone and City**: Bar chart with a facet wrap to show energy usage levels by city and climate zone 🏙️🌍
- **Energy Consumption by Appliances**: Bar chart showing energy consumption by different types of appliances 🍽️🔌

---

## Modeling 📐

### Linear Regression Models 🔍

- **Model 1**: Comprehensive model considering various predictors of energy consumption 🔄
- **Model 2**: Refined model focusing on significant variables such as average temperature and energy consumption by appliances 🌡️🍴
- **Final Model (Model 5)**: Simplified model with improved predictive power, focusing on key variables like average temperature, ceiling fans, cooling systems, and freezers 🌡️🌀

### Model Results 📊

- **Model 1**: Multiple R-squared value of 0.778, indicating 77.8% of the variability in total energy consumption is explained by the model 📉
- **Model 2**: Multiple R-squared value of 0.99, indicating 99% of the variability is explained, with significant predictors including ceiling fans, cooling systems, and freezers 🌬️❄️

---

## Shiny Apps 🌐

### Features 📲

- **Dashboard**: Includes a header, sidebar with a city filter, and boxes for displaying total current and future energy consumption 📈
- **Visualizations**:
    - Percentage distribution of usage levels by climate zone and city 🌍
    - Scatter plot of temperature vs. energy consumption 🌡️➡️⚡
    - Comparison of actual vs. predicted energy consumption per hour ⏱️

[Link to Shiny App](#)

---

<img width="675" alt="Screenshot 2025-02-05 at 11 10 08 PM" src="https://github.com/user-attachments/assets/95020278-843a-42dc-8550-a3f57820e1e1" />


## Strategies for Peak Energy Demand Management 🌞

### Demand Response Programs ⚡

- **Ceiling Fans**: 
  - Implement smart ceiling fan controls 🌬️
  - Offer incentives for reducing usage during peak hours 🌙
  
- **Exterior Lights**: 
  - Install motion sensors and timers 💡
  - Provide rebates for upgrading to energy-efficient LED fixtures 🌟

- **Freezers**: 
  - Implement load shifting to off-peak hours ⏰
  - Introduce peak time pricing to incentivize off-peak usage 💰

- **Fireplaces**: 
  - Install programmable thermostats to control heating more efficiently 🔥

---

## Conclusion 🎯

This project successfully addresses the challenges of peak energy demand by focusing on demand-side management strategies ⚡. By analyzing energy consumption patterns, implementing demand response programs, and engaging with the community, the project aims to reduce peak energy demand, improve grid reliability, and promote environmental sustainability 🌱🌍. The final model and Shiny app provide valuable tools for understanding and predicting energy consumption, enabling the energy company to make informed decisions and optimize energy usage during peak periods 🔋.

---

## Contact 📧

For questions or more information, feel free to reach out:

- **Project Team Lead** - email@example.com 📧
