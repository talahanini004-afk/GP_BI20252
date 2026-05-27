# Data Description and Understanding

## Dataset Overview

The dataset used in this project is a panel dataset covering Jordanian governorates between 2014 and 2024. Each row represents a governorate-year observation.

The dataset includes unemployment rate as the main target variable and multiple socioeconomic indicators as explanatory variables.

## Panel Data Structure

Panel data combines two dimensions:

- Cross-sectional dimension: Jordanian governorates.
- Time-series dimension: years from 2014 to 2024.

This structure allows the project to study both regional differences and changes over time.

## Target Variable

The target variable in this project is **Unemployment Rate**. It represents the percentage of unemployed individuals in the labor force.

This variable was selected because it directly measures the labor market problem being analyzed.

## Main Variables

| Variable | Description | Importance |
|---|---|---|
| Governorate | Name of the Jordanian governorate | Regional unit of analysis |
| Year | Observation year | Time dimension |
| Unemployment Rate | Percentage of unemployed individuals | Main target variable |
| Employment Rate | Percentage of employed individuals | Labor market indicator |
| Establishments per 1,000 people aged 15+ | Number of establishments relative to working-age population | Economic activity indicator |
| Population Density | Population per unit area | Demographic pressure indicator |
| Schools per 1,000 Population | Number of schools relative to population size | Education infrastructure indicator |
| Students per School | Average students per school | School capacity indicator |
| Students per Class | Average students per class | Classroom density indicator |
| Classes per School | Average classes per school | School infrastructure indicator |
| Student Ratio 5–19 | Student ratio in the school-age population | Education participation indicator |
| Labor Force | Economically active population | Labor market supply indicator |
| Employed | Number of employed individuals | Labor market outcome |
| Unemployed | Number of unemployed individuals | Labor market outcome |

## Selected Regression Features

The final regression model used three main explanatory variables:

- Establishments per 1,000 people aged 15 and above.
- Population Density.
- Schools per 1,000 population.

These variables were selected because they represent three important dimensions related to unemployment analysis:

- Economic activity.
- Demographic pressure.
- Educational infrastructure.

In addition, the selected variables were tested using the Variance Inflation Factor (VIF). The VIF results showed that these variables did not suffer from severe multicollinearity, meaning that they were suitable to be used together in the regression model.

## Clustering Features

The clustering analysis used a wider set of variables because the goal was not prediction, but grouping governorates according to socioeconomic similarity.

The clustering features included:

- Unemployment Rate.
- Establishments per 1,000 people aged 15 and above.
- Population Density.
- Students per Class.
- Schools per 1,000 Population.
- Student Ratio 5–19.

Including unemployment rate in clustering is acceptable because clustering is unsupervised analysis. In this context, unemployment rate was used as one socioeconomic characteristic among others, not as a prediction target.

## Initial Data Understanding

Initial exploration showed that unemployment patterns differ across governorates and years. Some governorates showed consistently higher unemployment rates, while others had more stable or lower values.

The data also suggested that socioeconomic indicators such as population density, establishments, and education indicators vary significantly across governorates. This variation supports the use of panel data models and clustering techniques.