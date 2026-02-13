# AB-Testing-Customer-Segmentation
Statistical A/B testing and K-Means clustering analysis for conversion optimization.


## Project Overview

This project evaluates whether a new marketing or website design improves conversion rates using A/B Testing.  
It also segments customers into behavior-based groups using K-Means Clustering.

The goal is to make data-driven marketing and product decisions.

##  Dataset Used

- File: stats.csv
- Key Columns:
  - user_id → Unique customer identifier
  - group → Control or Treatment group
  - converted → Conversion status (1 = Yes, 0 = No)

##  A/B Testing Analysis

### Hypothesis Setup
- H₀: No difference in conversion rate between Control and Treatment groups.
- H₁: Significant difference in conversion rate.

### Method Used
- Two-Sample Independent t-Test
- Significance Level (α) = 0.05

### Result
If p-value < 0.05 → The treatment has a statistically significant impact on conversion.

### Visualization
- Bar plot for average conversion rate
- Count plot for total conversions per group

## Customer Segmentation (K-Means Clustering)

### Steps Performed
- Selected numeric features
- Scaled features using StandardScaler
- Used the Elbow Method to determine optimal clusters
- Applied K-Means with k = 4
- Assigned each customer to a cluster

### Segment Insights
- Cluster 0 → Low engagement users
- Cluster 1 → High-value / loyal customers
- Cluster 2 → Moderate users (re-engagement opportunity)
- Cluster 3 → New or less active users

## Key Business Insights

- The A/B Test confirmed whether the new design improves conversion performance.
- K-Means clustering revealed distinct customer behavior patterns.
- Helps focus retention strategies on high-value segments.
- Supports data-driven marketing decisions.

##  Tools & Technologies Used

- Python, pandas, numpy, matplotlib, seaborn, scipy.stats, scikit-learn

##  Outcome

The analysis validates marketing effectiveness using statistical testing and identifies meaningful customer segments to optimize targeting strategies.
