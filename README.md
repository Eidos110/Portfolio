# Data Science Portfolio

Welcome to my portfolio! This repository showcases three projects that demonstrate my skills in data analysis, machine learning, and time-series forecasting. These projects solve real-world problems related to customer behavior, content classification, and sales forecasting.

## Projects Overview

### 1. Customer Segmentation & RFM Analysis
- **Objective**: Segment customers based on Recency, Frequency, and Monetary (RFM) metrics to enhance marketing strategies.
- **Techniques**: RFM scoring, KMeans clustering.
- **Key Insights**:
  - Segmented customers into groups (`Low`, `Mid`, `High Value`) with special focus on `Champions` and `Potential Loyalists`.
  - Found correlations among RFM metrics, suggesting targeted actions can enhance overall customer value.
  - The majority of customers fell into high-value segments, providing an opportunity to reinforce loyalty with targeted campaigns.

### 2. Predict Movie Genre
- **Objective**: Automate the classification of movie genres using plot summaries.
- **Techniques**: Natural Language Processing (TF-IDF), Logistic Regression, Decision Trees.
- **Key Insights**:
  - Identified genre-specific language patterns, helping differentiate genres like `drama` and `action`.
  - Logistic Regression achieved the highest accuracy (~64%), though overlapping themes made some genres challenging to distinguish.
  - Adding metadata (e.g., cast, director) could improve accuracy and better capture subtle differences between genres.

### 3. Promotion Time Series Forecasting
- **Objective**: Analyze and forecast the impact of promotional campaigns on sales.
- **Key Insights**:
  - **All stores & products sell more during promotions**no exceptions.
  - **Product 3** (most expensive, base price `~$20.70`) sees `~50%` price cuts during promotions and jumps from `88 → 400` avg. units sold.
  - **Store 10** is the top performer: `200,924` total units, `$1.76M` revenue.
  - **Holidays show no consistent sales lift** non-holiday weeks often outperform.
  - **Strong monthly seasonality** in Store 10 and Product 3.
- **Forecasting with Prophet**
  - **Target**: Weekly sales ( `Price × Weekly_Units_Sold`) for Store 10, Product 3
  - **Baseline model** (standard Prophet):
    - **RMSE = 1,190.10**
  - **Enhanced model**: Added two custom seasonalities:
    - `school_holiday_season (months 6–8)`
    - `not_school_holiday_season (rest of the year)`
  - **Result: RMSE = 1,125.73 (5.4% improvement)**
  - **Forecast horizon: 50 weeks ahead**
- **Techniques**
  - **Methods**: EDA with ECDFs & facet grids, feature engineering, time series decomposition, RMSE evaluation.
  - **Visualization**: Interactive Plotly line charts, Seaborn seasonal trends, Prophet component plots.

- **Why it Matters**
  - Debunks myth: Holiday = sales boost → false
  - Validates strategy: Promotional pricing is the real lever for demand
  - Enables planning: Accurate 50-week forecasts support inventory & pricing decisions for the highest-value segment



## Summary of Results
- **Customer Segmentation**: Enabled targeted marketing to maximize customer lifetime value.
- **Movie Genre Prediction**: Showed the potential and limitations of NLP in genre classification, with room for feature enhancement.
- **Sales Forecasting**: Provided valuable insights into the effectiveness of promotions and the timing of campaigns.

## Tools & Technologies
- **Languages**: Python
- **Libraries**: scikit-learn, pandas, matplotlib, Prophet, NLTK, Plotly, Seaborn
- **Tools**: Jupyter Notebook, GitHub

## About This Portfolio
Each project in this portfolio addresses a specific business problem—whether it’s understanding customer behavior, automating content classification, or optimizing sales strategies. This collection illustrates the power of data-driven insights in decision-making.

## License
Licensed under the [Apache-2.0 License](LICENSE).
