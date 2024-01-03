# python-api-challenge

# Weather Analysis - Overall Observations

## Temperature Variation

As anticipated, there is a noticeable temperature difference between the Northern and Southern Hemispheres. In the Northern Hemisphere, temperatures decrease as latitude increases (moving towards the North Pole), while in the Southern Hemisphere, temperatures tend to increase with higher latitudes.

## Humidity and Cloudiness

Latitude does not appear to exert a strong influence on humidity or cloudiness in the analyzed cities. The observed positive correlations are weak, suggesting that latitude alone may not be a significant predictor of these weather variables.

## Wind Speed

Latitude demonstrates a weak influence on wind speed, with a slight positive correlation in the Northern Hemisphere and a slight negative correlation in the Southern Hemisphere. This implies that latitude alone is not a robust predictor of wind speed.

## Notes

- The analysis relies on linear regression models, assuming a linear relationship between variables. Other unconsidered factors may contribute to the observed weather patterns.
- Scatter plots and regression lines serve as visual aids to represent relationships, with the R-value providing quantification of strength and direction of these relationships.


# Vacation Analysis

## Overview

This project involves the analysis of weather data for various cities, including temperature variation, humidity, cloudiness, and wind speed. Additionally, the project uses the Geoapify API to search for hotels near each city and visualizes the results on a map.

## Data Analysis

### Temperature Variation

As expected, there is a noticeable temperature difference between the Northern and Southern Hemispheres. The Northern Hemisphere experiences colder temperatures as latitude increases, while the Southern Hemisphere experiences warmer temperatures.

### Humidity and Cloudiness

Latitude does not seem to have a strong influence on humidity or cloudiness in the analyzed cities. The positive correlations are weak, indicating that latitude alone may not be a significant predictor of these weather variables.

### Wind Speed

Latitude also has a weak influence on wind speed, with a slight positive correlation in the Northern Hemisphere and a slight negative correlation in the Southern Hemisphere. This suggests that latitude alone is not a strong predictor of wind speed.

### Filtered Cities Based on Weather Conditions

The code filters cities based on specific weather conditions, including low humidity (< 50), low cloudiness (< 5), a maximum temperature between 290 and 310 Kelvin, and a wind speed greater than 5.5 m/s.

## Hotel Search

The Geoapify API is used to find the nearest hotel within 10,000 meters of each city's coordinates. The hotel names are stored in a new DataFrame (`hotel_df`), along with city, country, coordinates, and humidity.

## Map Visualization

The humidity map is visualized with points representing cities, and the size of each point corresponds to the humidity level. Hovering over a point on the map displays information such as city name, country, humidity, and hotel name (if available).

## No Hotel Found

The sample data in the `hotel_df` DataFrame shows "No hotel found" for each city. This could be due to issues with the Geoapify API request or the absence of hotels within the specified radius for the provided cities.

## Conclusion and Notes

The conclusions drawn are based on linear regression models and assumptions. The scatter plots and regression lines provide a visual representation of the relationships, and the R-value quantifies the strength and direction of these relationships.

It's important to note that the accuracy of these conclusions depends on the quality and representativeness of the data used in the analysis. The absence of hotels in the Geoapify API results may warrant further investigation or alternative approaches for obtaining hotel information.
