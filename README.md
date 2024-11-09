# Boston Housing Analysis

This project explores the factors affecting housing prices in Boston using statistical analysis and data visualization. By identifying key predictors of property value, this analysis provides insights that could be valuable for real estate investors, urban planners, and policymakers.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
4. [Visualizations](#visualizations)
5. [Key Findings](#key-findings)
6. [Conclusion and Implications](#conclusion-and-implications)
7. [How to Run the Project](#how-to-run-the-project)

## Project Overview

The Boston Housing Analysis project aims to answer:
- What are the main factors influencing housing prices in Boston?
- How do variables like crime rate, education quality, and neighborhood characteristics affect home values?
- Can we identify trends and patterns that would be useful for decision-making in real estate and urban planning?

Through data analysis and visualization, we uncover insights into how property values are shaped by various socioeconomic and environmental factors.

## Dataset

The dataset used in this analysis is the [Boston Housing Dataset](https://www.kaggle.com/datasets/vikrishnan/boston-house-prices), which includes details about homes in various Boston neighborhoods. Key variables include:
- **CRIM**: Crime rate per capita by town
- **ZN**: Proportion of residential land zoned for large lots
- **INDUS**: Proportion of non-retail business acres per town
- **CHAS**: Proximity to the Charles River (1 if close, 0 otherwise)
- **RM**: Average number of rooms per dwelling
- **AGE**: Proportion of owner-occupied units built before 1940
- **PTRATIO**: Pupil-teacher ratio by town
- **LSTAT**: Percentage of lower status population
- **MEDV**: Median value of owner-occupied homes in $1000s (target variable)

### File Location
The dataset file (`HousingData.csv`) is included in the `Data` folder.

## Methodology

The analysis process includes:
1. **Exploratory Data Analysis (EDA)**: Summary statistics and correlation heatmaps help identify relationships between variables and potential predictors of housing prices.
2. **Hypothesis Testing**: We examine relationships, such as between crime rate and median home price, to assess how neighborhood safety impacts property values.
3. **Regression Modeling**:
   - **Simple Linear Regression**: Examines the impact of the average number of rooms (`RM`) on housing prices (`MEDV`).
   - **Multiple Linear Regression**: Analyzes the combined effect of various predictors (`RM`, `LSTAT`, `PTRATIO`) on housing prices to improve the model's predictive power.

## Visualizations

To support our findings, we include a range of visualizations in `Boston_Housing_Analysis_Visualizations.ipynb`:
1. **Correlation Heatmap**: Highlights relationships among all features, showing which factors are strongly correlated with housing prices.
2. **Histogram of Home Prices**: Displays the distribution of `MEDV`, illustrating the range and central tendency of home values.
3. **Scatter Plot of Rooms vs. Price**: Demonstrates the positive correlation between the number of rooms (`RM`) and price.
4. **Box Plot of Prices by River Proximity**: Shows if proximity to the Charles River impacts home prices.
5. **Crime Rate vs. Price Scatter Plot**: Reveals how higher crime rates are associated with lower property values.
6. **Average Price by Pupil-Teacher Ratio (Bar Plot)**: Illustrates how educational quality influences property values.
7. **Socioeconomic Status (LSTAT) vs. Price (Box Plot)**: Examines the impact of socioeconomic status on property prices.

## Key Findings

1. **Room Count (RM)**: A positive correlation exists between the number of rooms in a home and its price, indicating that larger homes tend to be more valuable.
2. **Crime Rate (CRIM)**: Higher crime rates are associated with lower housing prices, emphasizing the importance of neighborhood safety.
3. **Socioeconomic Status (LSTAT)**: Higher percentages of lower status population negatively affect housing prices.
4. **Education Quality (PTRATIO)**: Areas with better pupil-teacher ratios command higher prices, which is an important factor for families.
5. **River Proximity (CHAS)**: Homes near the Charles River tend to have slightly higher prices, although this effect is less impactful than other variables.

## Conclusion and Implications

This analysis provides actionable insights into Boston’s housing market:
- **Real Estate Investors**: Can prioritize properties with larger rooms, low crime rates, and good school districts to maximize investment value.
- **Urban Planners**: Focusing on reducing crime and improving educational resources could enhance property values in various neighborhoods.
- **Homebuyers**: Families interested in quality education may find properties in areas with favorable pupil-teacher ratios more appealing.

Overall, the analysis confirms that factors like home size, neighborhood safety, socioeconomic status, and educational quality significantly affect Boston’s housing prices.