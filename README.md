# Analysis-on-Apartment-Prices
This project builds and evaluates a multiple linear regression model to identify key drivers of apartment prices across various countries. Using a dataset of over 147,536  property listings (original) and 22 predictors (e.g., total area, number of bathrooms, floor level, and country), the model helps uncover both feature-based and location-based influences on price

1. Business Request

To analyze and identify the key factors influencing apartment prices globally, especially in the post-COVID era, in order to support data-driven decision-making for real estate investment strategies.

2. Main Idea

This project uses multiple linear regression to explore the relationship between apartment features (such as size, number of bathrooms, floor level, etc.) and their prices across different countries. And the main goal is to determine which variables most significantly impact pricing and uncover country-level trends that may guide investment opportunities. Here are the variables: 

    Price_in_USD (Target Variable): Listing price of the apartment in US dollars.

    Country: Country where the apartment is located (used for one-hot encoding).

    Building_construction_year: Year the building was constructed.

    Building_total_floors: Total number of floors in the building.

    Apartment_floor: The floor on which the apartment is located.

    Apartment_total_area: Total area of the apartment (in square meters).

    Apartment_living_area: Living area of the apartment (in square meters).

    Apartment_bedrooms: Number of bedrooms in the apartment.

    Apartment_bathrooms: Number of bathrooms in the apartment.

3. Tools and Techniques Used

Tool:
  Python, with Pandas for data manipulation, Statsmodels for regression modeling, and Matplotlib for data visualization.
  
Techniques:

  Exploratory Data Analysis:
  
  - Investigated distributions, trends, and relationships between variables such as apartment size, number of rooms, construction year, and price.
  
  Data Cleaning and Preprocessing:
  
  - Removed missing and duplicate entries.
  
  - Extracted numerical values from area columns (e.g., removed “m²”).
  
  - Dropped nominal columns that were not useful for modeling.
  
  - Applied one-hot encoding to the country variable to convert categorical data into numerical format.
  
  Outlier Removal:
  
  - Used boxplots to identify and remove extreme values in price and area to improve model stability.

  Correlation Analysis:
  
  - Measured pairwise correlations between variables to identify strong relationships (e.g., between apartment size and number of bedrooms/bathrooms).
  
Modeling:
  
  Multiple Linear Regression (OLS):
  
  - Built an initial regression model to predict apartment prices using all relevant features.
  
  Backward Elimination:
  
  - Removed statistically insignificant variables (e.g., building_total_floors, apartment_bedrooms) to improve model interpretability and reduce multicollinearity.
  
  Country-Level Coefficient Interpretation:

  - Analyzed the impact of each country on apartment prices relative to Australia, identifying markets with significantly lower or statistically insignificant price differences.
