# Project Deployment Effort – Use Case

## Deployment Overview

The project can be deployed as a Business Intelligence solution that supports unemployment monitoring and labor market analysis in Jordan.

The main output is an interactive Tableau dashboard supported by a Python-based analytical pipeline.

## Main Use Case

The main use case is labor market monitoring for decision-makers. A user such as a policy analyst, researcher, or government employee can use the dashboard to understand unemployment trends and compare governorates.

The dashboard can help answer:

- Which governorate has the highest unemployment rate?
- How has unemployment changed over time?
- Which socioeconomic factors are associated with unemployment?
- Are there groups of governorates with similar labor market conditions?
- Which model gives the best analytical explanation?

## User Journey

A typical user journey would be:

1. The user opens the Tableau dashboard.
2. The user selects a specific year or governorate using filters.
3. The dashboard updates automatically.
4. The user reviews unemployment trends and geographic differences.
5. The user opens the factor dashboard to understand possible determinants.
6. The user refers to the report for statistical interpretation.
7. The user uses the insights to support decisions or further research.

## Deployment Options

The project can be deployed through:

- Tableau Public
- Tableau Server
- Scheduled PDF report
- GitHub repository
- Future Streamlit web application

## Project Workflow

```text
Raw Data Sources
↓
Excel Dataset
↓
Python Cleaning and Transformation
↓
Regression Modeling
↓
LOYO Validation
↓
PCA and Clustering
↓
Generated Figures and Outputs
↓
Tableau Dashboards
↓
Final Insights and Recommendations