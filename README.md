# Understanding Key Drivers of Residential Energy Consumption in Peak Month

## Overview
This project analyzes residential energy consumption patterns in South Carolina and parts of North Carolina, aiming to provide insights into reducing peak energy usage during extreme weather months. The study was conducted for eSC, a small energy company, to help mitigate energy demand spikes and avoid building new energy facilities.

## Problem Definition
Energy consumption tends to rise significantly during peak summer and winter months, particularly in July. The goal of this project is to predict energy consumption for a hypothetical July where hourly temperatures increase by 5°C. By leveraging historical consumption, housing attributes, and weather data, we aim to identify key drivers of energy usage and recommend strategies for incentivizing customers to reduce energy consumption.

## Data Sources
- **Housing Data**: Contains attributes for 5,710 homes, including square footage, cooling systems, and other structural characteristics.
- **Energy Data**: Includes 8,759 observations per home, capturing energy usage from various sources on an hourly basis for all months in 2018.
- **Weather Data**: Provides 8,760 hourly weather observations for 46 counties, detailing temperature, humidity, wind speed, and solar radiation.

## Key Business Questions
1. Which sources of energy contribute most to overall consumption?
2. How does energy consumption vary between the hottest and coldest counties?
3. Does HVAC system type (Heat Pump vs. Central AC) impact cooling energy usage?
4. How does home size influence energy usage for lighting and plug loads?
5. Do temperature increases affect energy consumption trends for major contributors?

## Exploratory Data Analysis (EDA)
- **Feature Selection**: Reduced the original 171 house attributes to 93 meaningful features.
- **Energy Consumption Trends**: Identified key contributors such as cooling energy, interior lighting, and plug loads.
- **Correlation with Weather**: Found a strong relationship between rising temperatures and increased energy consumption, particularly in cooling energy.

## Modeling Approach
- **Energy Source Analysis**: Identified cooling, plug loads, and lighting as top contributors.
- **Cooling Energy Models**: Explored variations in cooling energy consumption across different counties.
- **HVAC System Impact**: Analyzed the relationship between HVAC types and energy consumption.
- **Square Footage Effects**: Investigated the role of home size in energy consumption patterns.
- **Predicting Energy Demand in Hotter Conditions**: Created models to forecast increased demand with rising temperatures.

## Model Performance
- **Cooling Energy Model**: R² = 0.3714
- **Lighting Energy Model**: R² = 0.2145
- **Plug Load Model**: R² = 0.7518 (most predictive model)
- Found that every 1°C increase in temperature leads to a 0.052 kWh increase in energy usage for cooling, lighting, and plug loads.

## Key Insights & Recommendations
1. **Smart Plugs & Light Timers**: Providing customers with automated controls can help reduce unnecessary consumption.
2. **Smart Thermostats**: Encouraging optimized temperature settings based on occupancy and peak demand times.
3. **Target High-Usage Homes**: Implementing interventions for the most energy-intensive households.
4. **Experimental Evaluation**: Conducting controlled studies to measure the impact of smart devices on energy savings.

## Conclusion
By understanding and predicting energy consumption patterns, eSC can proactively implement strategies to manage peak demand, improve efficiency, and reduce the need for costly new power plants. The project highlights actionable insights for influencing customer behavior and optimizing energy consumption.

