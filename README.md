📊 Netflix Top 10 Performance Analysis
📌 Overview

This project analyzes Netflix Top 10 weekly performance data to uncover relationships between audience ratings, engagement metrics, ranking position, and content longevity. The objective was to apply structured data cleaning, predictive modeling, and exploratory analysis to derive actionable insights about content performance dynamics.

The dataset contains 500+ records with variables such as weekly rank, cumulative weeks in the Top 10, weekly hours viewed, IMDb rating, runtime, and category.

🧹 Data Cleaning & Preprocessing

The dataset included missing values across key metrics. Different imputation strategies were applied based on the nature of each variable:

Weekly Hours Viewed → Random Forest regression (to handle skewed engagement distribution)

IMDb Rating → Regression-based imputation

Runtime → Category-level median imputation (content-based attribute)

Removed unrealistic predicted values using logical validation thresholds

This approach ensured structural consistency while preserving business realism.

📈 Exploratory Data Analysis

Key analyses included:

Rank vs Weekly Hours Viewed

IMDb Rating vs Longevity in Top 10

Engagement distribution across categories

Runtime distribution by content type

Correlation matrix of numerical features

Visualizations were built using Matplotlib to highlight performance patterns and engagement concentration.

🔍 Key Insights

Strong inverse relationship between weekly rank and viewing hours

Engagement is highly concentrated among top-ranked titles

Higher-rated titles tend to remain longer in the Top 10

Runtime shows weak correlation with engagement

English TV titles drive a significant portion of platform engagement

🛠 Tools & Technologies

Python

Pandas

NumPy

Matplotlib

Scikit-learn (Linear Regression, Random Forest)

🎯 Business Relevance

This analysis demonstrates how audience perception, ranking mechanics, and engagement metrics interact — providing insight into:

Content investment strategy

Engagement concentration risk

Viewer retention patterns

Data-driven performance evaluation
