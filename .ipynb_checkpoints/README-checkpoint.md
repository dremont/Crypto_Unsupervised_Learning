# Crypto Unsupervised Learning 

# Description

The goal of this project is to create a jupyter notebook that clusters cryptocurrencies by their performance in different time periods using unsupervised learning to help identify potential investment opportunities. 

# Libraries and Dependencies

import pandas as pd
import hvplot.pandas
from pathlib import Path
from sklearn.cluster import KMeans
from sklearn.decomposition import PCA
from sklearn.preprocessing import StandardScaler


# Resources

You will need the following csv from the resources file: crypto_market_data.csv.

# Overview

After importing libraries, dependencies, and reading in dataframe we plot and scale our data to prepare it for 
analysis. We then run the KMeans module to cluster the different cryptos. After this we make use of an Elbow Curve to identify if we have used the optimal amount of clusters. We then use the PCA module to see if we can further optimize these clusters as well as check our conclusions with an additional elbow curve. 

# Conclusion

I managed to effectively cluster the data into 4 groups which will greatly assist in quickly identifying investment opportunities. One finding is that using the PCA method did not drastically reduce the number of clusters. After visually analyzing there is not major change between the KMeans clusters of the original dataframe compared to the PCA. 