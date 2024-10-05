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

### 3. Promotional Time Series Analysis
- **Objective**: Analyze and forecast the impact of promotional campaigns on sales.
- **Techniques**: Prophet model for time-series forecasting.
- **Key Insights**:
  - Promotions led to significant sales increases, especially for Product 3 and Store 10, highlighting effective discount strategies.
  - Seasonal trends were found across products and stores, with sales peaking during holidays.
  - Time-series forecasting with the Prophet model effectively captured sales trends and provided actionable predictions, especially when holiday seasonality was considered.

## Summary of Results
- **Customer Segmentation**: Enabled targeted marketing to maximize customer lifetime value.
- **Movie Genre Prediction**: Showed the potential and limitations of NLP in genre classification, with room for feature enhancement.
- **Sales Forecasting**: Provided valuable insights into the effectiveness of promotions and the timing of campaigns.

## Tools & Technologies
- **Languages**: Python
- **Libraries**: scikit-learn, pandas, matplotlib, Prophet, NLTK, Plotly
- **Tools**: Jupyter Notebook, GitHub

## About This Portfolio
Each project in this portfolio addresses a specific business problem—whether it’s understanding customer behavior, automating content classification, or optimizing sales strategies. This collection illustrates the power of data-driven insights in decision-making.

## License
Licensed under the [Apache-2.0 License](LICENSE).
