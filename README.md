# Portfolio



### **A.	BUSINESS UNDERSTANDING PROJECT**

Project Predict Movie genre
-	Discover the captivating world of movies, a beloved form of entertainment enjoyed by millions worldwide. In this age of abundant streaming services and burgeoning websites, imagine the incredible potential of a predictive model that effortlessly identifies the genre of a movie based solely on its plot summary. By harnessing the power of technology, this groundbreaking approach has the power to significantly reduce the laborious task of manually tagging movies. Embrace the future of cinema organization and experience the countless benefits of automated genre generation.


Project Customer Segmentation & RFM Analysis
-	Understanding customers and tailoring strategies to their needs is crucial for success. RFM analysis segments customers based on recency, frequency, and monetary value, helping you target valuable customers. With our project, gain insights into customer behavior and identify patterns to create targeted campaigns and personalized offers. Reward loyal customers and optimize pricing, inventory, and product offerings. Identify at-risk customers with RFM analysis, retain them, and increase customer lifetime value. Uncover hidden patterns, make data-driven decisions, and optimize your business strategies with our project. Don't miss out on understanding your customers and unlocking growth opportunities


Project Promotional Time Series
-	Analyzing promotional activities is crucial for business success. This project uses time-series data to provide insights into the effectiveness of promotions. With Project Promotional Time Series, understand the correlation between promotions and key metrics. Uncover optimal timing, duration, and nature of campaigns to maximize impact. Predict future outcomes and make data-driven decisions to allocate resources effectively. Empower your business to drive growth and increase profitability with this project. Don't miss out on unlocking new opportunities - harness the power of data to propel your business to new heights


### **B.	RESULT SUMMARY**

Project Predict movie genre
-   The modified plot using tfidf provides better performance during modeling.
-   GridSearchCV helps narrow down the values of the best model's hyperparameters.
-   The model with the best performance is the logisticRegression model on the plot modified using tfidf with the following parameters:
  C = 1.0, class_weight = 'None', multi_class = 'multinomial', penalty = 'l2', solver = 'lbfgs'
- 	When the above model is used on the test set, it achieves an accuracy score of around 64%, which is a significant improvement from the baseline.
- 	The Confusion Matrix confirms what I suspected when looking at common words in those genres.
- 	Because some genres have the same words as other genres, false predictions for those genres mainly occur in genres with similar words.
- 	The decision tree model has the least favorable performance



Project Customer Segmentation & RFM Analysis
- 	The goal of this project is to perform RFM analysis using unsupervised methods to solve the problem.
- 	The model used is KMeans with the following parameters:
    n_cluster = 3, init='k-means++', n_init=10, max_iter=300, random_state=111, algorithm='elkan'
- 	In the recency part, cluster 1 and 3 have almost the same values, while cluster 3 has significantly higher values.
- 	In the frequency part, cluster 1 and 2 have the same values, while cluster 2 has the highest value.
- 	In the MonetaryValue part, the values are almost the same as the Frequency part.
- 	Overall, cluster 1 has stable values in each part.



Project Promotional Time Series
- 	This case is related to sales with a focus on the effect of having or not having promotions.
- 	To solve this problem, we use Time Series techniques. Then we use the Prophet model.
- 	Most stores have some seasonal patterns and they record the highest sales around July.
- 	Each product has a regular price and a promotional price. There is no significant difference between the regular price and the promotional price for Product 1 and Product 2, but the promotional price   for Product 3 can be reduced by 50% from its original price. Although every store offers discounts for this product, Store 10 has the highest sales during the discount period.
- 	It is not surprising that sales are higher during promotions compared to regular days. Store 10 makes Product 3 the best-selling product around July.

