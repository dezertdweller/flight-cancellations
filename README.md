# Predicting Flight Delays & Cancellations
*Capstone Project Proposal by Katia Lopes-Gilbert*

## Problem Space
How might we leverage historical flight performance and weather data to enable airlines and passengers to make more informed decisions and reduce the impact of flight delays on travel plans?

## Context
Flight delays have significant economic and logistical impacts, costing the aviation industry billions of dollars annually. Delays affect both airline operations and passenger satisfaction, often leading to cascading effects such as missed connections, rebookings, and logistical complications. This project aims to predict the likelihood of flight delays and cancellations based on historical flight performance data and weather conditions. Accurately forecasting delays will enable airlines, airports, and passengers to take proactive measures, minimizing disruptions and enhancing decision-making for all involved.

## Criteria for Success
* Achieve 85% accuracy in forecasting flight delays exceeding 15 minutes and cancellations.
* Develop a model that can handle multivariate data sources, including flight schedules and weather.
* Provide actionable insights that airlines and passengers can use in real time or during pre-flight planning.

## Scope of Solution Space
This project will focus on the top 20 airports with the highest flight volumes in 2023. By narrowing the scope to these key airports, we will obtain consistent and robust data, ensuring that the model captures relevant trends without being overwhelmed by smaller, less significant routes. Each airport will be analyzed using flight data (including schedules, actual departure/arrival times, and delay/cancellation data) and hourly weather data.

## Constraints
* Data availability: While flight performance data is available monthly, weather data may vary in granularity and completeness across different locations.
Computation limits: Processing large datasets from multiple sources, especially weather and flight data, could be computationally intensive.
* Temporal scope: The dataset is limited to flight performance and weather data from 2023, and external factors such as policy changes or sudden operational disruptions may affect predictions.

## Stakeholders
* Airline passengers: Benefiting from improved travel plans, real-time alerts, and potentially fewer disruptions.
* Airline operation staff: Gaining operational insights to optimize scheduling, resource allocation, and delay management.
* Airport traffic control: Ensuring better coordination and resource management in anticipation of delays.
* Travel booking sites (Kayak, Expedia, Booking, etc.): Providing users with more accurate delay forecasts and improving user experience.

## Data Sources
1. Department of Transportation
* Monthly airline performance data for 2023: Available as .csv files, this data will provide flight schedules, on-time performance, and delay/cancellation information.
* Annual aircraft registration data: Available as a .csv file, containing detailed information on aircraft types and registration, which may be relevant to predicting delays based on aircraft age or model.

2. Weather data for top 20 airports:
* Hourly weather data for each airport will be sourced from public repositories. This data will include variables like temperature, wind speed, precipitation, and visibility, all known to affect flight performance.

## Deliverables
1. **Exploratory Data Analysis (EDA) Report:** A detailed analysis of trends in flight delays and cancellations across the top 20 airports. This report will include visualizations of delay patterns, seasonality, and correlations with weather conditions.
2. **Predictive Model:** A trained machine learning model capable of forecasting flight delays exceeding 15 minutes and cancellations based on flight performance and weather data. Model evaluation metrics such as accuracy, precision, recall, and F1-score will be provided.
3. **Final Project Report:** Comprehensive documentation outlining the problem, data sources, methodology, model performance, and key insights from the analysis. Recommendations for how airlines, passengers, or travel platforms could implement the findings.

