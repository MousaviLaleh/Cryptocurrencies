# Cryptocurrencies


## Analysis Overview
The purpose of this project is to use unsupervised machine learning to analyze a database of cryptocurrencies and create a report including the traded cryptocurrencies classified by group according to their features.
This classification report could be used by an investment bank to propose a new cryptocurrency investment portfolio to its clients.<br/>

We use the following methods for the analysis:
 - Preprocessing the database.
 - Reducing the data dimension using Principal Component Analysis.
 - Clustering cryptocurrencies using K-Means.
 - Visualizing classification results with 2D and 3D scatter plots.

## Resources
Data :&nbsp; [cryptoData.csv](Resources/crypto_data.csv) 
<br/>
Software :&nbsp;  [Python 3.7.7](https://www.python.org/downloads/),&nbsp; [Anaconda 1.9.12](https://www.anaconda.com/)

## Results
Following the preprocessing and cleaning phase we have a total of 532 tradable cryptocurrencies.

### Clustering Cryptocurrencies using K-Means - Elbow Curve
We don't know what would be the output of the analysis so we are using unsupervised machine learning to identify clusters of the cryptocurrencies. We produced the elbow curve below using the K-Means method iterating on k values from 1 to 10.

<p align="center"><img src="Resources/01.png"></p>

<br/>
The best k value appears to be 4 so we would conclude on an output of 4 clusters to categorize the crytocurrencies.

<br/>

### Visualizing Cryptocurrencies Results

### 3D-Scatter plot with clusters

<p align="center"><img src="Resources/02.png"></p>

<br/>
This 3-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to three principal components.


### Tradable Cryptocurrencies Table

<p align="center"><img src="Resources/03.png"></p>

<br/>
Most of the cryptocurrencies are part of class #0 and #3. <br/>
The snapshot below shows that BitTorrent is the only cryptocurrency in class #2. <br/>

<p align="center"><img src="Resources/04.png"></p>


### 2D-Scatter plot with TotalCoinMined vs TotalCoinSupply

<p align="center"><img src="Resources/05.png"></p>

<br/>
Plotting the scatter plot from two cryptocurrency features directly does not efficiently segregate the different classes. Then using the PCA algorithm is the right method for better visualizations.

## Summary
We have identified the classification of 532 cryptocurrencies based on similarities of their features. <br/>
Particularities of each group need to be analyzed to determined their performance and potential interest for the investment bank's clients.

