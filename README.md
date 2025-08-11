# Analyzing-Customer-Purchase-Behavior

RFM Segmentation: Customers were successfully segmented into four RFM clusters based on their Recency, Frequency, and Monetary values. Due to the nature of the dummy PurchaseDate (all '2023-01-01'), Recency and Frequency were consistent across customers, with the main differentiation being the Monetary value.
Cluster 0 exhibited the highest average Monetary value ($90.55).
Cluster 3 had the second highest average Monetary value ($70.50).
Cluster 1 had the third highest average Monetary value ($50.50).
Cluster 2 had the lowest average Monetary value ($29.97).
Lack of Temporal Data: A significant limitation was identified in the PurchaseDate column, which contained only a single date ('2023-01-01'). This prevented meaningful time-series analysis (trends, seasonality, anomalies) and cohort/retention analysis beyond the initial purchase cohort.
Basket Analysis Impeded: No meaningful association rules could be generated from the basket analysis. This was likely due to the dataset structure, where each customer appeared to have only a single purchase record, making it impossible to identify co-purchased items within transactions.
Age and Purchase Amount Relationship: A hypothesis test (Pearson correlation) found no statistically significant linear relationship between Age and Purchase Amount (p-value = 0.515 > 0.05).
Univariate Distributions: Visualizations of individual feature distributions (Recency, Frequency, Monetary, AOV, Tenure) were generated, showing their spread and frequency, although the dummy date limited the variability of Recency, Frequency, and Tenure.
Bivariate Relationships: Scatter plots and a correlation matrix were generated to explore relationships between numerical variables. The correlation matrix showed the strength and direction of linear relationships between Recency, Frequency, Monetary, AOV, and Tenure.
Insights or Next Steps
The primary differentiator for customer segmentation in this dataset, given the data limitations, is the Monetary value. Focus on analyzing customer attributes associated with higher spending clusters (0 and 3).
Obtaining or generating a dataset with actual purchase dates spanning a realistic period is crucial for performing meaningful time-series analysis, cohort analysis, and a more accurate RFM analysis that reflects true customer behavior over time.
