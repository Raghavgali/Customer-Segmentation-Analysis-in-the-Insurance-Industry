# Customer-Segmentation-Analysis-in-the-Insurance-Industry

## Project Overview

This project investigates customer segmentation within an insurance dataset to identify distinct groups of customers based on their product interests, market participation, and responsiveness to marketing. The ultimate goal is to optimize strategic decisions regarding marketing promotions, pricing strategies, and targeted customer outreach.

## Problem Statement

We aim to segment customers in the insurance industry to identify various groups with distinct behaviors. These insights will help businesses tailor marketing strategies to optimize promotions, pricing, and targeted efforts, improving customer satisfaction and profitability.

## Dataset

	•Size: 10,290 rows and 13 columns.
	•Missing Values: Approximately 2% missing values.
	•Target Variable: Lifetime Value = (Annual profit from the customer) x (Number of years they are a customer) - (Acquisition cost).

## Data Preprocessing

	•Handling Missing Values: Imputed continuous variables using the mean and categorical variables using the mode.
	•Outlier Removal: Outliers were treated using IQR and manual thresholding techniques.
	•Feature Engineering: New features were added using custom formulas to enhance data interpretability and scalability. Features like education were categorized numerically to aid analysis.
	•Scaling: Min-Max Scaler provided the most optimal results in terms of clustering.

## Clustering Methods

We applied various clustering algorithms, including:
	•K-Means
	•Hierarchical Clustering
	•Gaussian Mixture Models
To evaluate the clustering performance, we used the Silhouette Score, and further parameter optimization was performed using GridSearchCV for the best clustering solution.

## Key Customer Segments

	1.Young Educated Adults with Low Purchasing Power: Customers in this segment contribute high premiums but at low retention costs.
	2.Seniors with No Children and High Purchasing Power: High monthly incomes, educated, with a low percentage of claim rates.
	3.Middle-Aged Profitable Customers: Middle-class salaries with the lowest claims rate and highest motor premiums.
	4.Oldest Customers with No Children and High Purchasing Power: Highest monthly income and high health premium contributors.
	5.Middle-Aged Customers with Medium Purchasing Power: Average income, largest spenders in motor premiums, with varying product interests.

## Strategic Insights

	•Focus on middle-aged customers for standard insurance plans.
	•Target young adults with basic insurance plans and retirement adults with premium insurance offerings.
	•Cross-sell products to high-spending customers.
	•Allocate marketing budgets carefully to less profitable segments.

## Notebooks & Scripts

The USML_mid_final.ipynb notebook contains the complete implementation of the project.
	•EDA: Exploratory Data Analysis including handling missing values, outliers, and feature engineering.
	•Clustering: Detailed implementation of different clustering algorithms, including K-Means and Hierarchical Clustering.
	•Model Performance: Evaluation metrics for clustering solutions.
	•Visualization: Detailed visualizations of the customer segments and key insights.

## Conclusion

Through clustering, we identified actionable customer segments that help drive the insurance company’s marketing and product strategies. These insights provide a clear pathway to targeting high-value customers and improving retention strategies, while reducing losses from less profitable segments.
