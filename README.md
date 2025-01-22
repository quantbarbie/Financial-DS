# Analyst Coverage Data Analysis

This project explores analyst coverage data, focusing on similarity analysis, clustering, and dimensionality reduction. The steps below outline the methodology and insights gained.

---

## 1. Data Import and Exploration
- **Dataset**: `Analyst_Coverage.csv` containing fields such as:
  - Analyst Name
  - Broker
  - Rating
  - Recommendation
  - Target Price
  - Company Ticker (BBTICKER)
  - Sector
  - Industry Group
- **Exploration**:
  - Inspected dataset structure and content using `.head()`, `.tail()`, `.describe()`, and `.value_counts()`.
  - Identified numeric fields (e.g., `RATING`, `TARGET_PRICE`) and categorical fields (e.g., `SECTOR`, `INDUSTRY_GROUP`).

---

## 2. Preprocessing
- **Handling Missing Data**:
  - Checked for null values and missing entries.
  - Imputed missing values for numeric fields using median values.
  - Dropped rows with missing critical categorical data.
- **Categorical Encoding**:
  - Converted categorical fields (e.g., `BROKER`, `RECOMMENDATION`) into numerical representations using one-hot encoding.

---

## 3. Similarity Analysis
- **Objective**: Determine the similarity of brokers based on their ratings and recommendations.
- **Approach**:
  - Constructed pairwise similarity matrices using cosine similarity on encoded fields.
  - Visualized similarity relationships using heatmaps.

---

## 4. Dimensionality Reduction
- **Objective**: Reduce dataset dimensionality for better visualization and clustering.
- **Approach**:
  - Applied **Principal Component Analysis (PCA)** to reduce the data to 2D and 3D components.
  - Visualized reduced dimensions using scatter plots.

---

## 5. Clustering
- **Objective**: Identify clusters of brokers and analysts based on their rating patterns.
- **Approach**:
  - Applied K-means clustering on reduced dimensions.
  - Determined the optimal number of clusters using the **elbow method**.
  - Visualized clusters in 2D and 3D space.

---

## 6. Insights and Observations
- Identified groups of brokers with similar rating behavior.
- Highlighted clusters of analysts sharing similar recommendations within sectors and industry groups.
- Found correlations between analyst coverage patterns and market sectors.

---

## 7. Future Work
- Incorporate time-series analysis of analyst ratings.
- Explore the influence of specific brokers on target price trends.
- Evaluate the impact of ratings on stock price performance.

---


