# CryptoClustering
This challenge combines Python programming skills with unsupervised learning skills 
The data provided contains information of price change of cryptocurrencies over a period of time, in csv format.
Listed below are the steps performed on this data
- Import Data (provided in the starter code)
- Prepare Data (provided in the starter code)
- Find the best value for k Using the original Data
- Cluster Cryptocurrencies with K-means Using the original Data
- Optimize clusters with Principal Component Analysis
- Find the Best Value for k Using the PCA Data
- Cluster the Cryptocurrencies with K-means Using the PCA Data
- Visualize and Compare the Results


# Technologies used
Scikit-learn - machine learning tools for unsuoervised data analysis.
Tools - Cluster, StandardScaler, Preprocessing, Decomposition and hvplot

# Overview of the Analysis 


Raw data

![image](https://user-images.githubusercontent.com/119769357/236115430-faeabaea-c4e6-4d41-9141-8c6750af6da9.png)


We find different levels of inertia associated with different number of clusres(k) using K-Means to create an elbow plot. Concluded that k=4 is the best choice after visual inspection.

![image](https://user-images.githubusercontent.com/119769357/236115977-76102131-216f-4579-ae40-8feeb52ecb98.png)


Using the optimal k value to train and predict the K-Means model to generate 4 clusters of cryptocurrencies. The inertia of each cluster was significant enough to consider reducing the amount of features.

![image](https://user-images.githubusercontent.com/119769357/236116491-b8e29b2c-9a3f-4672-91fb-dffbc62282b0.png)


Applying the Principal Component Analysis to create 3 primary clusters and re-calculating the optimal value of k using the PCA data using the elbow curve

![image](https://user-images.githubusercontent.com/119769357/236117145-9633ce79-d816-4f16-b080-104a877da731.png)

This elbow curve also determines the best value for k as 4 
Here is the plot that incorporates the PCA data

![image](https://user-images.githubusercontent.com/119769357/236117600-15129060-a9e7-46e2-b135-9c3daaefac30.png)

# References
Data for this dataset was generated by edX Bootcamps LLC, and is intended for educational purposes only.
