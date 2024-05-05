# Exploratory Data Analysis for Songs

This code performs an exploratory data analysis (EDA) on a dataset of songs to guide the model building process. The EDA includes data preprocessing, checking for duplicates, missing values, and anomalies. It explores the distributions of variables, temporal patterns, and relationships between features and the target variable "copies_sold".

Key findings:
- Only ~6% of songs sold above 2 million copies, suggesting a regression approach over classification.
- The number of songs released per year is decreasing, with the Folktronica genre consistently releasing the most songs.
- Bands produce songs within the same genre, allowing for a hierarchical modeling approach.
- No strong evidence of seasonality in song releases.
- Interaction effects observed between energy, loudness, and length with respect to copies sold.

The code proposes two modeling strategies:
1. Random forest regression to predict if a new song will sell more than 2 million copies.
2. Time series approach using an autoregressive model or a regression model with fixed effects for genre and year to evaluate genre popularity.

The EDA provides insights into the data and informs the feature engineering process for building predictive models.
