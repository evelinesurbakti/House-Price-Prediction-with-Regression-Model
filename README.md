# House Price Prediction with Regression Model

The data **House.csv** contains information on the sale of 76 single-family homes in Dublin during 2005. We will model single-family home sale price by (Price in thousands of eur/100,000), which range from 155.5 (155,500 Euros) to 450.0 (450,000 Euros), using these predictor variables:

- __Size__ floor size (thousands of square feet)
- __Lot__ lot size category (from 1 to 11 explained below)
- __Bath__ number of bathrooms (with half-bathrooms counting as 0.1 explained further in the report)
- __Bed__ number of bedrooms (between 2 and 6)
- __Year__ year the house was built.
- __Garage__ garage size (0, 1, 2, or 3 cars)
- __High__ indicator for The High School (reference: The High School)
- __Alexandra__ indicator for Alexandra College (reference: Alexandra College)
- __Stratford__ indicator for Stratford College (reference: Stratford College)
- __St.Mary's__ indicator for St.Mary's College (reference: St.Mary's College)
- __St Louis__ indicator for St Louis High School (reference: St Louis High School)

It seems reasonable to expect that homes built on properties with a large amount of land area command higher sale prices than homes with less land, all else being equal. However, an increase in land area of (say) 2000 square feet from 4000 to 6000 should probably make a larger dierence (to sale price) than going from 24,000 to 26,000. Thus, realtors have constructed lot size \categories," which in their experience correspond to approximately equal-sized increases in sale price.


| Lot Size      | Category        | 
| ------------- | --------------- | 
| 1             | 0-3000ft2       | 
| 2             | 3000-5000ft2    | 
| 3             | 5000-7000ft2    | 
| 4             | 7000-10,000ft2  | 
| 5             | 10,000-15,000ft2| 
| 6             | 15,000-20,000ft2| 
| 7             | 20,000ft2-1 acre| 
| 8             | 1-3 acres       | 
| 9             | 3-5 acres       | 
| 10            | 5-10 acres      | 
| 11            | 10-20 acres     | 

To reflect the belief that half-bathrooms (i.e., those without a shower or bath-tub) are not valued by home-buyers nearly as highly as full bathrooms, the variable Bath records half-bathrooms with the value 0.1.

## Main Goal
We want to model single-family home sale price using these predictor variables:

### Data Set
Dataset included (House.csv). The data contains information on the sale of 76 single-family homes in Dublin during 2005.

Introduction 
Exploratory Data Analysis 
  Distribution of Sales Prices of the Houses
  How Sales Prices vary based on the Categorical Variables 
  How Sales Prices vary based on the Numerical Variables 
Regression Model
  Multiple Linear Regression Model 
  The Intercept
  The βsize 
  The βBath1.1
  The Effect of Predictor Variable Bed 
  Significant Predictor Variables
  Values those lead to Largest and Lowest Expected Value of the House Prices 
  Residuals of the Expected Value of the House Prices
  Adjusted R-squared value 
  F-Statistic 
ANOVA
  Type 1 Anova
  Type 2 Anova
Diagnostics 
  Linearity 
  Random/i.i.d
  Multicollinearity
  Zero Conditional Mean and Homoscedasticity
  Normality
Leverage, Influence and Outliers 
  Leverage  
  Influence  
  Outliers  
Expected Value, CI and PI

## Document format
This project is written in Rstudio, and knitted to .docx. 

We are using R version 4.0.2 and ggplot version 3.3.2
