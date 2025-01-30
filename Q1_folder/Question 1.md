# K-Means Clustering for Customer Segmentation

## Dataset:
Credit card clustering dataset: https://www.kaggle.com/datasets/arjunbhasin2013/ccdata/data
The dataset has been downloaded and added to the main branch of github.

## Explanation 

To address the customer segmentation problem, K-Means Clustering is chosen as the traditional, non-neural network approach. This method is widely used for customer segmentation tasks because it groups customers with similar behaviour or characteristics. K-Means is particularly well-suited for numerical datasets like the one provided, 
where continuous variables such as balances, purchases, and frequency of transactions are prevalent.

One of the main advantages of K-Means is its ease of interpretation. Since the algorithm creates clusters based on proximity in feature space, it is straightforward to explain the characteristics of each group, such as identifying high spenders, frequent payers, or instalment-focused customers. Moreover, K-Means is computationally efficient 
and can handle large datasets, such as the 9,000 customers in this case. The algorithm assumes that clusters are spherical and equidistant, which works well with financial datasets after appropriate preprocessing and normalization.

To apply K-Means clustering, the first step is preprocessing. This includes handling missing data through imputation (such as mean imputation for MINIMUM_PAYMENTS and CREDIT_LIMIT), normalizing the data to prevent features with larger ranges from dominating the clustering process, and selecting relevant features like BALANCE, PURCHASES, CREDIT_LIMIT, and PAYMENTS.
Next, the optimal number of clusters is determined using methods such as the Elbow Method or Silhouette Analysis. Once the number of clusters is selected, the K-Means algorithm is used to divide the customers into groups. The final step is interpreting the results by examining the centroid values to understand the characteristics of each customer segment.

The performance of K-Means clustering can be evaluated using metrics like the Silhouette Score, which measures how well-separated the clusters are, and Inertia, which calculates the sum of squared distances of samples to their nearest cluster centre. These metrics provide insights into the quality of the clusters formed. However, challenges with K-Means include 
its sensitivity to the initialization of centroids and its inability to handle overlapping or non-spherical clusters.

When compared to other traditional approaches such as Hierarchical Clustering, DBSCAN, and Gaussian Mixture Models (GMM), K-Means is a simpler and faster option, especially when the data forms well-separated spherical clusters. In contrast, Hierarchical Clustering can be computationally expensive for large datasets, and DBSCAN may not perform well with
high-dimensional data. GMM offers more flexibility but is less scalable and harder to interpret. Ultimately, K-Means provides a straightforward solution for customer segmentation and helps inform marketing strategies effectively.
