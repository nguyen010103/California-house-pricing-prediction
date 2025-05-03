# California-house-pricing-prediction

This project uses the California Census housing dataset to median home values based on features like population, location, and house characteristics.

---

## Goals 
- Explore the dataset and understanding the data trend.
- Train machine learning models to predict house prices.
- Create visualizations
- Publish results and code in a clean, reproducible format.

--- 

## Features Analysis Summary

### Median Income
- The distribution is right-skewd, meaning the most housholds were earning below average income in the dataset.
- Income is positively correlated with house value.

### Housing Age
- The distribution is fairly uniform.
- Not very informative on its own.

### Correlation Heat Map
- Median_income has a strong positive linear relationship - use a core predictor.
- Avg_rooms and avg_bedrooms have low correlation with the house value - combine for better use.
- Combining latitude and longitude via clustering.
- Consider dropping population and average_occupants to reduce noise.

### Latitude and Longitude
- Generate California house price per location.

--- 

## Engineered dataset
- Combine avg_rooms and avg_bedrooms because both of them had a high correlation to each other. Using both will be redundant.
- Drop the column due to low or near zero correlation with the house median price: populations, avg_bedrooms and avg_rooms