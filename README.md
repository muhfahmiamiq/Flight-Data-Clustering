# Flight Data Clustering

## 1. Business Problem

The airline industry faces numerous challenges in customer retention, personalized marketing, and service optimization. Understanding customer behavior and preferences is crucial to tailor services, enhance loyalty programs, and optimize routes and schedules. Clustering this customer dataset can aid in identifying distinct customer segments based on their behaviors, preferences, and value to the airline.

## 2. Solution Strategy

My approach revolves around employing clustering techniques to gain insights into customer behavior within the airline industry. By leveraging clustering algorithms, the aim is to segment customers into distinct groups based on similarities in their travel patterns, preferences, loyalty engagement, or other pertinent attributes.
1. EDA: Exploratory Data Analysis (EDA) involves using descriptive statistics and both univariate and multivariate analysis methods to understand the dataset's attributes, intending to explore and grasp its nature.
2. Data Preprocessing: Selecting features for clustering in a business context, it's essential to consider attributes that align with the business objectives or could potentially reveal valuable insights. Preparing raw data for machine learning models involves a crucial stage known as data preprocessing. This phase encompasses various activities focused on cleaning, transforming, and structuring the data to render it appropriate for analysis or modeling purposes.
3. Modelling & Evaluation: Modeling and evaluating data using K-means clustering involves initially determining the best number of clusters through methods like the elbow technique or silhouette scores. Once the optimal cluster count is identified, visualization techniques, like scatter plots, help interpret the resulting clusters, while silhouette scores quantify the quality of clustering, ensuring a robust analysis and pattern recognition.
4. Model interpretation + Recommendations: Interpreting clusters in a business context involves grasping their unique traits for targeted strategies. By understanding these clusters, tailored recommendations can optimize services or marketing efforts, aligning business actions with the specific needs and behaviors identified within each group.

## 3. Modeling & Evaluation

1. Elbow Method
![Screenshot 2023-12-06 221720](https://github.com/muhfahmiamiq/Flight-Data-Clustering/assets/148199919/533d7257-d8bf-4a7a-b94c-96d7aac25f6f)
From the percentage above, the largest decrease in inertia percentage occurred between 1 cluster and 2 clusters (40.76% - 23.87% = 16.89%). So the optimal cluster is 2

2. K-Means Clustering
![Screenshot 2023-12-06 221817](https://github.com/muhfahmiamiq/Flight-Data-Clustering/assets/148199919/286fd333-8915-498d-ad44-a77c01a5464a)
clustering visualization results using K-means

3. silhouette score
![Screenshot 2023-12-06 221938](https://github.com/muhfahmiamiq/Flight-Data-Clustering/assets/148199919/4266fdc2-4d37-4368-9b1e-43ac540cbd56)
n_clusters with the highest silhouette_score value is 2 with a value of 0.518818905286916. Therefore, the optimal number of clusters for this data is 2. The reason is because the highest silhouette_score value indicates that the objects in that cluster match each other better compared to other clusters.

![Screenshot 2023-12-06 222014](https://github.com/muhfahmiamiq/Flight-Data-Clustering/assets/148199919/521b6ba2-eae2-44a8-a0a1-2f88a8a5ae90)
From the graph above, it is also evident that the optimal number of clusters is 2

## 4. Model interpretation + Recommendations
Interpretation:
1. Cluster 0: Customers in this cluster are, on average, slightly younger with a lower average income and shorter total flying distance compared to Cluster 1. They travel less frequently and may pay more attention to airfare.

2. Cluster 1: Customers in this cluster are, on average, slightly older with a higher average income and longer total flying distance compared to Cluster 0. They travel frequently and may be more prepared to spend more on airline tickets.

Recommendation:
Recommendations for Cluster 0:
1. Special Offers: Since customers in this cluster tend to have lower first- and second-year ticket revenues, consider providing special offers or promos that can encourage them to spend more. This could be a special discount, an incentive from a loyalty program, or a customized travel package.
2. Services for Youth: Since customers in this cluster tend to be younger, it may be a good idea to tailor services to better suit the tastes of young travelers. This could include offering more affordable prices, flexibility in travel arrangements, or interaction via social media.

Recommendations for Cluster 1:
1. Premium Service: Customers in this cluster tend to spend more and travel longer distances. Consider presenting premium services, such as exclusive lounges, priority boarding, or special amenities to satisfy their desires and encourage loyalty.
2. Rewards for frequent travelers: Considering customers in this cluster often travel long distances, they would probably be happy with a frequent flyer program. Enhance and promote your loyalty program, including rewards like free flights, class upgrades or exclusive experiences for frequent travelers.
