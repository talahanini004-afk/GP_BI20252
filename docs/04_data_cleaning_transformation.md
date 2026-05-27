# Data Primary Cleaning and Transformation

## Introduction

After understanding the dataset structure, the next stage was data cleaning and transformation. This stage was necessary because raw data collected from different official sources may contain inconsistent column names, missing values, different formats, and variables with different scales.

The purpose of this stage was to transform the raw dataset into an analysis-ready panel dataset. Python was used as the main tool for cleaning, transformation, feature selection, validation, and exporting processed outputs.

## Data Cleaning Process

The data cleaning process included several steps:

- Importing the Excel dataset into Python.
- Standardizing column names.
- Removing extra spaces from governorate names.
- Converting numeric columns into numeric data types.
- Handling missing values.
- Creating derived indicators.
- Selecting relevant features.
- Standardizing variables for clustering.
- Exporting cleaned data and results.

## Column Renaming

The raw dataset contained column names with spaces, symbols, and inconsistent formatting. Therefore, the columns were renamed into clean Python-friendly names.

Examples:

| Original Column Name | Cleaned Column Name |
|---|---|
| Governorates | Governorate |
| YEAR | Year |
| Unemployment Rate | Unemployment_Rate |
| Population Density | Population_Density |
| Schools per 1,000 population | Schools_per_1000_population |
| Establishments per 1,000 (15+) | Establishments_per_1000_15plus |
| Students per Class | Students_per_Class |

## Data Type Conversion

Numeric variables were converted into numeric data types because some values may be imported from Excel as text.

This step was important because regression models, clustering algorithms, and statistical calculations require numeric input.

## Handling Missing Values

Rows with missing values in essential modeling variables were removed from the modeling dataset.

The project did not remove data randomly. Only observations missing essential variables such as governorate, year, unemployment rate, or selected regression features were removed to ensure model stability and valid results.

## Derived Indicators

A very important part of the data preparation stage was the creation of derived variables. Some required indicators were not directly available in the raw data, so they had to be calculated using formulas.

For the years 2014–2016, the dataset did not provide the actual number of population by some age categories. Instead, the available data provided population rates or percentages. Therefore, the project team calculated the actual population values using total population and the available percentage rate.

For example, the population aged 15 and above was calculated using the following Excel formula:

```excel
=Table3[@[Total Population]]*(Table3[@[population +15 Rate]]/100)