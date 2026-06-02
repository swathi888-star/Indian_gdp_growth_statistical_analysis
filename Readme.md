# GDP Growth Variability Analysis - India (IMF WEO Dataset)

## Project Overview
This project investigates the key macroeconomic drivers behind India's GDP growth variability over the last four decades (1980–2024). Using data from the IMF's World Economic Outlook, this analysis explores the relationships between GDP growth and primary economic indicators: **Total Investment**, **Inflation**, and **Export Volume**.

## Objectives
- Identify key drivers of India’s economic "speed."
- Analyze the volatility and long-term stability of major economic indicators.
- Quantify the impact of Investment on GDP growth using statistical modeling and machine learning.

## Key Insights
- **Investment as a Catalyst:** Investment is identified as the primary driver of growth. Statistical analysis confirms that high-investment regimes significantly increase the probability of high GDP growth (from a 50% baseline to 73%).
- **Economic Trinity:** PCA reveals a tight "cluster" between GDP, Investment, and Exports, indicating they move in sync during periods of expansion.
- **The 2020 Anomaly:** The analysis identifies the 2020 pandemic-induced contraction as a structural break, handled through robust median-based statistics to ensure baseline stability.
- **Inflation Trade-off:** There is a persistent "heating up" risk, where high growth and investment often tension against inflation, highlighting the importance of maturing monetary policy.

## Technical Stack & Methodology
- **Data Source:** IMF World Economic Outlook (WEO).
- **Processing:** Data cleaning, transposition (melt/pivot), and feature engineering using `Pandas`.
- **Statistical Analysis:**
    - Descriptive Statistics (Mean, Median, IQR, Outlier detection).
    - Inferential Statistics (T-tests, One-way ANOVA, Chi-Square tests).
    - Probability (Bayes' Theorem for conditional probability).
- **Visualization:** `Seaborn` & `Matplotlib` (Histograms, Boxplots, Line Trends, Correlation Heatmaps).
- **Machine Learning:** Principal Component Analysis (PCA) for dimensionality reduction and understanding economic "heartbeats."

## Project Structure
- `data/`: (If applicable) Raw and processed datasets.
- `notebooks/`: Jupyter Notebook containing the full analysis code.
- `reports/`: Detailed project documentation and PDF summary.

## Limitations
- **Lag Effects:** The model currently focuses on same-year impacts; future iterations could incorporate time-lagged variables.
- **Sample Size:** Limited by annual data points; robust statistical corrections (T-distribution, Yates' Correction) were applied to mitigate small sample size constraints.

---
*Project No. 36 | Submitted by: Swathi Sathyanarayana*