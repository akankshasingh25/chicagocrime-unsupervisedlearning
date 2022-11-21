# Unsupervised Learning on Chicago Crime Dataset 
### Introduction:
The Chicago Police department keeps an up-to-date record of crimes taking place from 2001 till date. This data can be used for predictive analysis to gain a better understanding of the crimes taking place in Chicago. The dataset is available on Chicago Data Portal which has about 7 million data points and 22 columns [[Crimes - 2001 to Present | City of Chicago | Data Portal]](url). 

### Aim:
In this project, 100k data points with 22 categorical features namely ID, Case number, Date, Block, IUCR, Description, Primary type, Location description, Arrest, Domestic, Beat, District, Ward, Community Area, FBI Code, X Coordinate, Y Coordinate, Year, Updated On, Latitude, Longitude, Location were considered. So far, the Chicago crime data has been used for supervised learning to predict crime, arrest and data analysis. To the best of our knowledge, no previous attempt has been made to perform unsupervised learning on the crime data. This project is an attempt to identify natural clusters in the data and features contributing to the formation of clusters.

### Experiment:
The dataset being huge and as only few features showed correlations, preprocessing and feature engineering was an important task here to reduce the complexity of the data. As the data is categorical in nature, a major difficulty was to find an algorithm that takes categorical variables as input. For this, the alternative of K-Means: K-Modes was explored. The challenge here was to specify the number of clusters(k). By data exploration and intuition, we assumed the number of clusters as 31 which is the number of unique categories in the feature ”Primary Type”. Another model explored was Spectral clustering which doesn’t require the number of clusters to be specified by the user. 

### Results:
The Normalised Mutual Information (NMI) score for both these models were calculated. Based on this score, Spectral Clustering was seen to perform better on our dataset.
