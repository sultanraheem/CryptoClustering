# CryptoClustering

# Visualize and Compare the Results

This section is not showing the graphs on GitHub, reason is unsure, this is what they look like in my Notebook Below

![image](https://github.com/user-attachments/assets/5a9f34a9-3260-4842-b237-20368f247527)

# Preparing Data 

Use the StandardScaler() module from scikit-learn to normalize the data from the CSV file.

Create a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

The first five rows of the scaled DataFrame should appear as follows:

# Find the Best Value for k Using the Original Scaled DataFrame

Use the elbow method to find the best value for k using the following steps:

Create a list with the number of k values from 1 to 11.
Create an empty list to store the inertia values.
Create a for loop to compute the inertia with each possible value of k.
Create a dictionary with the data to plot the elbow curve.
Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.
Answer the following question in your notebook: What is the best value for k?

# Cluster Cryptocurrencies with K-means Using the Original Scaled Data

Use the following steps to cluster the cryptocurrencies for the best value for k on the original scaled data:

Initialize the K-means model with the best value for k.
Fit the K-means model using the original scaled DataFrame.
Predict the clusters to group the cryptocurrencies using the original scaled DataFrame.
Create a copy of the original data and add a new column with the predicted clusters.
Create a scatter plot using hvPlot as follows:
Set the x-axis as "price_change_percentage_24h" and the y-axis as "price_change_percentage_7d".
Color the graph points with the labels found using K-means.
Add the "coin_id" column in the hover_cols parameter to identify the cryptocurrency represented by each data point.

# Optimize Clusters with Principal Component Analysis

Using the original scaled DataFrame, perform a PCA and reduce the features to three principal components.

Retrieve the explained variance to determine how much information can be attributed to each principal component and then answer the following question in your notebook:

What is the total explained variance of the three principal components?
Create a new DataFrame with the PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

The first five rows of the PCA DataFrame should appear as follows:

# Find the Best Value for k Using the PCA Data

Use the elbow method on the PCA data to find the best value for k using the following steps:

Create a list with the number of k-values from 1 to 11.
Create an empty list to store the inertia values.
Create a for loop to compute the inertia with each possible value of k.
Create a dictionary with the data to plot the Elbow curve.
Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.
Answer the following question in your notebook:
What is the best value for k when using the PCA data?
Does it differ from the best k value found using the original data?
Cluster Cryptocurrencies with K-means Using the PCA Data
Use the following steps to cluster the cryptocurrencies for the best value for k on the PCA data:

# Initialize the K-means model with the best value for k.

Fit the K-means model using the PCA data.
Predict the clusters to group the cryptocurrencies using the PCA data.
Create a copy of the DataFrame with the PCA data and add a new column to store the predicted clusters.
Create a scatter plot using hvPlot as follows:
Set the x-axis as "PC1" and the y-axis as "PC2".
Color the graph points with the labels found using K-means.
Add the "coin_id" column in the hover_cols parameter to identify the cryptocurrency represented by each data point.
Answer the following question:
What is the impact of using fewer features to cluster the data using K-Means?

# Any shots missing from the loading page when landing on Notebook

![image](https://github.com/user-attachments/assets/de31f7fa-113e-4cc4-9f25-3a580874a984)

![image](https://github.com/user-attachments/assets/5c9e0aab-c580-48ed-8ed2-26d6062821e1)

![image](https://github.com/user-attachments/assets/cf5cf163-ede3-433b-89a1-b352ffb26c8f)

![image](https://github.com/user-attachments/assets/ef283674-b85e-41e3-835c-5572f4efd1ab)

![image](https://github.com/user-attachments/assets/b805a907-9bb9-4f91-82e1-e3520a58ca04)

![image](https://github.com/user-attachments/assets/dc97d588-597f-4f80-b273-a8250d068ffb)

# Work Cited

https://chatgpt.com/share/a0a94dab-bb13-4320-ae16-8b36a2ed3474
