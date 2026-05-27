# Data-Driven Analysis of Unemployment in Jordan (2014–2024)

This graduation project analyzes unemployment in Jordan and its socioeconomic determinants using Python, panel data regression, Fixed Effects, VIF, PCA, clustering, and Tableau dashboards.

## Authors

- Tala Al-Hanini
- Majd Alqahwaje

## Supervisor

Dr. Husam Barham

## University

University of Petra – Faculty of Administration

## Course

307498 – Graduation Project  
Second Semester, 2025/2026

## Project Overview

This project focuses on analyzing unemployment patterns across Jordanian governorates from 2014 to 2024. The study combines Business Intelligence, statistical modeling, and machine learning techniques to identify socioeconomic factors associated with unemployment.

The project uses official Jordanian data sources, including the Jordan Department of Statistics, the Social Security Corporation, and the Ministry of Education.

## Project Structure

```text
graduationproject/
├── README.md
├── docs/
│   ├── 01_project_description.md
│   ├── 02_data_research.md
│   ├── 03_data_description.md
│   ├── 04_data_cleaning_transformation.md
│   ├── 05_visualization_insights.md
│   ├── 06_dashboard_design.md
│   ├── 07_advanced_analytics_modeling.md
│   ├── 08_tools_selection.md
│   ├── 09_deployment_use_case.md
│   ├── 10_results.md
│   └── 11_references.md
│
├── data/
│   ├── raw/
│   │   └── GRADUATION.xlsx
│   └── processed/
│       ├── cleaned_panel_data.xlsx
│       ├── descriptive_statistics.xlsx
│       ├── vif_results.xlsx
│       ├── model_comparison.xlsx
│       ├── leave_one_year_out_results.xlsx
│       ├── leave_one_year_out_predictions.xlsx
│       ├── cluster_profiles.xlsx
│       ├── cluster_governorate_averages.xlsx
│       ├── governorates_with_clusters.xlsx
│       ├── pooled_coefficients.xlsx
│       ├── pooled_residual_diagnostics.xlsx
│       ├── fixed_effects_base_coefficients.xlsx
│       ├── fixed_effects_coefficients_detailed.xlsx
│       └── fixed_effects_residual_diagnostics.xlsx
│
├── src/
│   └── ROUND2.py
│
├── notebooks/
│   └── code_example.ipynb
│
├── dashboards/
│   ├── Graduation.twb
│   ├── dashboard_1_labor_market_overview.png
│   └── dashboard_2_key_factors_affecting_unemployment.png
│
├── images/
│   ├── clustering_elbow_method.png
│   ├── clustering_silhouette_scores.png
│   ├── fe_actual_vs_predicted.png
│   ├── fe_residuals.png
│   ├── fixed_effects_base_coefficients.png
│   ├── governorates_clusters_pca.png
│   ├── hierarchical_dendrogram.png
│   ├── loyo_actual_vs_predicted.png
│   ├── loyo_residuals.png
│   ├── pooled_actual_vs_predicted.png
│   └── pooled_residuals.png
│
├── reports/
│   ├── final_report.docx
│   ├── final_report.pdf
│   └── final_presentation.pptx
│
├── models/
│   └── model.txt
│
├── requirements.txt
└── .gitignore