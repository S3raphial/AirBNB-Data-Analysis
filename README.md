# AirBNB-Data-Analysis
### STAT362 Final Project

This project analyzes an Airbnb listing data set, with the primary focus on exploring the key factors that influence prices across a few major U.S. cities. This project involved data cleaning, EDA, variable relationships, and predictive modeling using Random Forests and Linear Regression.

---

## Analysis Breakdown

This project was completed in 5 parts:

**Part 1**: Overview of the Dataset and key variable selection.  
**Part 2**: Data Cleaning  
**Part 3**: Univariate Exploration of 'log_price', 'room_type', and 'review_scores_rating'  
**Part 4**: Variable Relationship EDA between predictors and 'log_price'  
**Part 5**: Predictive Modelling, evaluation, and conclusions.   

---

## Results of Modeling

| Model | Test RMSE | Test R² |
|-------|-----------|---------|
| Linear Regression | 0.486 | 0.548 |
| Random Forest | 0.469 | 0.580 |

The Random Forest has lower RSME and larger R^2, which suggests nonlinear relationships between predictors and 'log_price'.

Some Key Findings:
- Room Type is the strongest predictor, as listings of an entire residence depand a premium over private or shared rooms.
- Size Variables('accommodates', 'bedrooms', 'bathrooms') have a strong positive correlation with price.
- Location matters significantly aswell, a potential reflection of the respective city's housing market or simply demand for listings.

## Data
This analysis was done using the Airbnb dataset found on:  
https://www.kaggle.com/datasets/lovishbansal123/airbnb-data  

## How to Run this Project
To replicate, ensure you have a working installation of R, and an IDE like RStudio is recommended.  

**R packages used:**
 
```r
install.packages(c("tidyverse", "knitr", "dplyr", "ggplot2", "randomForest"))
```
