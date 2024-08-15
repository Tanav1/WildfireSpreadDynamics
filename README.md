# Wildfire Spread Dynamics

## Project Summary
This project investigates the dynamics of wildfire spread in the northeast region of Portugal. The focus is on understanding the relationship between the Fine Fuel Moisture Code (FFMC) and the Initial Spread Index (ISI), which are crucial indicators of fire behavior. The analysis aims to determine how FFMC influences the speed at which wildfires spread.

## Methodology
- **Data Source:** The "Forest Fires" dataset from the UCI Machine Learning Repository, consisting of 517 instances with 13 features related to climate and physical factors in the Montesinho natural park.
- **Data Preparation:** The dataset was split into an exploration set (30%) and a confirmation set (70%). Outliers were detected and removed to ensure data quality.
- **Modeling Approach:**
  - A simple linear regression model was initially used to explore the relationship between FFMC and ISI.
  - A log-linear regression model was then applied to address skewness in the data and improve model fit.

## Key Results
- The log-linear regression model showed a strong relationship between FFMC and ISI, with an adjusted R² of 0.74.
- The log transformation improved model stability and linearity, providing a better fit compared to the simple linear model.
- FFMC was found to be a significant predictor of wildfire spread, as measured by ISI.

## Conclusion
The findings suggest that FFMC is a robust indicator for predicting the speed of wildfire spread in the studied region. The results highlight the importance of monitoring FFMC to assess wildfire risks, which could aid in better fire management and prevention strategies.

## References
- Howard, B. C. (2023, October 4). _How to live with mega-fires: Portugal’s forests may hold the secret_. National Geographic. Retrieved from [National Geographic](https://www.nationalgeographic.com/science/article/how-to-live-with-mega-fires-portugal-forests-may-hold-secret)
- Sampson, L. (2024, July 18). _Where are the Portugal wildfires and is it safe to travel?_. The Times. Retrieved from [The Times](https://www.thetimes.com/travel/advice/where-are-the-portugal-wildfires-is-it-safe-to-travel-ttflwnmnr)
