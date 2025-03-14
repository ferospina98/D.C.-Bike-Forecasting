# D.C.-Bike-Forecasting
Forecasting analysis for bike usage in Washington D.C.

This project analyzes and forecasts bike demand in Washington, D.C., using machine learning models. By leveraging data from Capital Bikeshare, we aim to understand the impact of time, seasonality, and ride types on bike usage.

The final model provides accurate demand predictions, helping bikeshare providers optimize fleet management and station availability.

## Dataset
Source: Capital Bikeshare Data
Time Period: January - December 2024
File Format: .csv (one file per month)

Key Features:
- Trip Details: ride_id, rideable_type, started_at, ended_at
- Station Information: start_station_name, end_station_name, start_lat, start_lng
- Rider Type: member_casual (Member vs. Casual Riders)

 ## EDA Findings
 1. Higher demand on weekdays , peaking during morning (7-9 AM) and evening (5-7 PM) rush hours.
 2. Spring & Summer months show the highest bike usage.  Winter months see a decline.
 3. Electric bikes have shorter trip durations, while classic bikes dominate overall usage.
 4. Dockless electric bikes introduce unpredictable demand patterns and were excluded from modeling.

## Machine Learning Model
We trained an XGBoost Regressor to predict bike demand based on:
- start_hour ⏰ (Time of day)
- start_weekday 📅 (Day of the week)
- start_month 📆 (Seasonality)

## Future Improvements
- Incorporate weather data to enhance predictions.
- Implement real-time demand forecasting for dynamic bike allocation.
- Explore deep learning models for further accuracy improvements.

## Conclusions
This project provides a data-driven approach to managing bikeshare operations efficiently. The insights help optimize bike redistribution, station planning, and commuter experience. 
