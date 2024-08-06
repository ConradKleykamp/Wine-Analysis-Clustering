# Wine-Analysis-Clustering
Employing unsupervised learning techniques to cluster a dataset

![image](https://github.com/user-attachments/assets/8e403c5c-aa83-458a-8249-d3b6d6608771)

---

### Objective
This project was completed as part of CU Boulder's Unsupervised Algorithms in Machine Learning course. The project attempts to demonstrate various clustering techniques along with dimensionality reduction. A dataset containing three different wines in the same region will be grouped via their 13 physicochemical characteristics. The data will first be scaled and then will have its dimensionality reduced through the use of principal component analysis (PCA). Following this, the data will be clustered into three groups via the use of k-means and t-SNE clustering algorithms. The dataset is adapted from UCI's Wine Data Set and is licensed for public use under the CC BY 4.0 license. 

---

### Methods
Libraries Used
- numpy
- pandas
- seaborn
- matplotlib
- sklearn (StandardScaler, PCA, KMeans, TSNE)

Exploratory Data Analysis (EDA)
- Histograms visualizing the distributions of each of the 13 wine characteristics
- Box plots visualizing the distributions of each characteristic
- Heatmap visualizing potential feature correlation

Data Preprocessing
- Scaling the data with StandardScaler
- Applying PCA, n_components = 2

Identifying Optimal Number of Clusters
- Elbow Method, n_clusters = 3
- Dendogram further showing the optimal number of clusters

Models
- k-means
- t-SNE

---

### General Results
- PCA --> 2 principal components captured 55.41% of the variance of the data
- k-means --> grouped the data into 3 clusters based upon the first and second principal components
- t-SNE --> grouped the data into 3 clusters based upon the first and second t-SNE components

In conclusion, both k-means and t-SNE successfully grouped the data into three clusters, thus correctly identifying three groups of wines. However, the positions of the clusters varied between each algorithm. This is likely due to the fact that k-means grouped the clusters based upon the first and second principal components, while t-SNE grouped its clusters based upon its own first and second t-SNE components. 
