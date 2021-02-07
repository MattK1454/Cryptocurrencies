# Cryptocurrencies Grouping Analysis

## Overview

The purpose of this project was to collect information on current cryptocurrencies and analyze said data for any patterns where cryptocurriences might be grouped
together to form an investment portfolio.

## Results

Due to the nature of the data collected and no real targeted variable of interest for grouping of the currencies, the data collected was run through an
unsupervised learning model using the KMeans algorithm to allow for the formation of clusters of currently trading cryptocurrencies that might act as a
bases for the development of an investment portfolio. 

![Cleaned cryptocurrency data](https://github.com/MattK1454/Cryptocurrencies/blob/main/Resources/images/cleaned_crypto_data.png)

The table presented above shows the final data after filtering for actively traded coins, coins with working algorithms, the primary component analysis 
(PCA) of each of those coins, and which grouping or class in which the coins is placed. The table contains 533 rows with 9 colums for each row. 
The first ten coins in the table are shown here. 

![Cryptocurrency table](https://github.com/MattK1454/Cryptocurrencies/blob/main/Resources/images/cryptotrading_hv_table.png)

This table shows similar information to the previous table but removes the PCA to allow for the grouping(class) aspect of each coin to become more 
prominent.

![Elbow curve for clustering determination](https://github.com/MattK1454/Cryptocurrencies/blob/main/Resources/images/KMeans_elbow_curve.png)

This graph is used to determine the approximate number of clusters optimal for clustering the data. As shown above, the slope of the line changes the 
most at point 4. This indicates 4 clusters would be the optimal target for this data.

![3D scatter plot of the Primary Component Analysis of cryptocurrency data](https://github.com/MattK1454/Cryptocurrencies/blob/main/Resources/images/PCA_3D_scatter_plot.png)

This plot was generated to show how each coin was plotted with respect to the PCA. The colors further act to distinguish which to group each coin 
belongs.

![Scatter plot of cryptocurrency data and groupings](https://github.com/MattK1454/Cryptocurrencies/blob/main/Resources/images/cryptotrading_plot.png)

This image is the 2 dimensions plot of where each coin is plotted with respect to "Total Coins Mined" and "Total Coin Supply". Each coin is also colored 
with respect to which group the coin falls into according to the PCA analysis to help review how each group as a whole also measures in regards to 
each other for "Total Coins Mined" and "Total Coin Supply".

# Summary

Reviewing the results above, the data was clustered into four groups. Three of the groups can be used for the foundation of developing a cryptocurrency 
investment portfolio. The fourth group is an outlying cryptocurrency (BitTorrent) from the others and therefore should not be included in a portfolio 
of investments. There is also the TurtleCoin currency in class 2 capable of being remove to further reduce the variation of investment in the class 2 
portfolio.

## References

1. Module 18 Challenge. (n.d.). Retrieved February 06, 2021, from https://courses.bootcampspot.com/courses/453/assignments/6659