# Cryptocurrencies
# Analysis Overview
The purpose of this project is to use unsupervised machine learning to analyze a database of cryptocurrencies and create a report including the traded cryptocurrencies classified by group according to their features.
This classification report could be used by an investment bank to propose a new cryptocurrency investment portfolio to its clients.</br>
We use the following methods for the analysis:</br>
</br>
* preprocessing the database,
* reducing the data dimension using Principal Component Analysis,
* clustering cryptocurrencies using K-Means,
* visualizing classification results with 2D and 3D scatter plots.

# Results
Following the preprocessing and cleaning phase we have a total of 532 tradable cryptocurrencies.


# Clustering Cryptocurrencies using K-Means - Elbow Curve
We don't know what would be the output of the analysis so we are using unsupervised machine learning to identify clusters of the cryptocurrencies.</br> 
We produced the elbow curve below using the K-Means method iterating on k values from 1 to 10.
![image](https://user-images.githubusercontent.com/95143562/166342324-3a0faf32-93e6-4a9e-9fdd-b12c8e369bd7.png)</br>
The best k value appears to be 4 so we would conclude on an output of 4 clusters to categorize the crytocurrencies.

# Visualizing Cryptocurrencies Results
<b>3D-Scatter plot with clusters</b></br>
![image](https://user-images.githubusercontent.com/95143562/166342368-5c1757de-adcd-46c1-994a-ed1b768da123.png)</br>
This 3-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to three principal components.

<b>2D-Scatter plot with clusters</b></br>
![image](https://user-images.githubusercontent.com/95143562/166342424-784d0504-f2a6-44a4-8bf2-507e4f9d3d8f.png)
</br>
This 2-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to two principal components.

Both these scatter plots show the distribution and the four clusters of cryptocurrencies.
We can identify the outliers like the unique cryptocurrency in the class #2.

<b>Tradable Cryptocurrencies Table</b>
![image](https://user-images.githubusercontent.com/95143562/166342624-31de5fc7-7390-4fef-9590-80d90f564498.png)

Most of the cryptocurrencies are part of class #0 and #1.
The snapshot above shows that BitTorrent is the only cryptocurrency in class #2.

<b>2D-Scatter plot with TotalCoinMined vs TotalCoinSupply</b>
![image](https://user-images.githubusercontent.com/95143562/166342650-cd624aeb-7b64-4fda-afa4-2d3ddde88536.png)

Plotting the scatter plot from two cryptocurrency features directly does not efficiently segregate the different classes. Then using the PCA algorithm is the right method for better visualizations.

# Summary
We have identified the classification of 532 cryptocurrencies based on similarities of their features.
Particularities of each group need to be analyzed to determined their performance and potential interest for the investment bank's clients.
