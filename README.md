# ML-Kaggle-Challenge---KNN-Imputation

This project focuses on the ```eBird Dataset``` which is the world's largest citizen science project. Often citizen scientist forget about some species they observed in the field when submitting their checklist that leads to missing data. Hence, through using KNN, it recommends species that are most likely to be observed so that the citizen scientist can double-check their checklists.

## Normalization ##

Firstly, the **training** and **test** dataset are normalized using the ```min-max log normalization``` Before trying the min-max log normalization, log normalization and  z-score normalization was used too. However, min-max log normalization provides us a good result.

## Distance Measure ##

Secondly, to measure the distance between two vectors, **3** different distance measured was used:

1. Euclidean Distance
2. Manhattan Distance
3. Cosine Distance

Among the three of them ```Manhattan Distance``` scored better in determining the distance between vectors.

The formula and function for all the 3 distance measure can be found in the Rmd file. 


## Approach ##

To determine, the k-nearest neighbor, Manhattan distance was used to calculate the distance between each training column set to each test set column and we received the matrix of **6009 \* 14832** The reason for choosing the K-nearest neighbor algorithm in comparison to the k-means was because the k-means initially chooses the centroid of cluster randomly which may not provide accurate recommendation.



