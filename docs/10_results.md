# Results

## Model Comparison Results

The project compared Pooled OLS, Fixed Effects, and Leave-One-Year-Out validation.

| Model | R² | RMSE | MAE | Interpretation |
|---|---:|---:|---:|---|
| Pooled OLS | 0.281 | 3.586 | 2.955 | Baseline model with limited explanatory power |
| Fixed Effects | 0.847 | 1.657 | 1.306 | Strongest in-sample model |
| Leave-One-Year-Out | 0.692 | Add from output | Add from output | Tests temporal generalization |

The Fixed Effects model achieved the strongest performance. This confirms that governorate-specific differences are important in unemployment analysis.

## Pooled OLS Result

The Pooled OLS model was useful as a baseline model. However, its performance was limited because it does not control for governorate-specific characteristics.

## Fixed Effects Result

The Fixed Effects model performed significantly better than Pooled OLS. This means that regional differences between governorates play an important role in explaining unemployment rates.

## LOYO Validation Result

Leave-One-Year-Out validation showed acceptable temporal generalization. This indicates that the model was not only fitting the training data but also predicting unseen years reasonably well.

## Clustering Results

The clustering analysis selected two clusters as the best grouping structure. This result was supported by the Elbow Method and Silhouette Score.

The clustering results showed that Jordanian governorates can be grouped according to socioeconomic similarity.

## Dashboard Results

The Tableau dashboards successfully presented the project findings visually.

Dashboard 1, Labor Market Overview, showed unemployment trends, governorate differences, and geographic distribution.

Dashboard 2, Key Factors Affecting Unemployment, showed the relationship between unemployment and socioeconomic variables such as population density, establishments, and schools.

## Key Findings

- Unemployment patterns differ significantly between Jordanian governorates.
- Fixed Effects regression is more suitable than Pooled OLS for this panel dataset.
- Governorate-specific characteristics are important in explaining unemployment.
- Economic establishments are important indicators of economic activity.
- Population density may reflect pressure on the labor market.
- Educational infrastructure may be related to labor market outcomes.
- Clustering revealed two main socioeconomic patterns among governorates.
- PCA improved the visualization of multidimensional clustering results.
- Tableau dashboards improved communication and decision support.

## Recommendations

- Labor market policies should consider governorate-specific differences.
- Governorates with high unemployment rates should receive targeted economic development programs.
- Investment and small business support should be encouraged in areas with limited job opportunities.
- Education programs should be better aligned with labor market needs.
- Government institutions should use Business Intelligence dashboards to monitor unemployment trends continuously.