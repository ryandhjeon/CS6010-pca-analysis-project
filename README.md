# Reflection

In this assignment, we used the following clustering algorithms: KMeans, Agglomerative, and Spectral. 

In addition, based on the conditions of fitting a model in SkLearn with these algorithms, we decided to proceed with using five scalars: StandardScalar, MinMaxScalar, Normalizer(L1), Normalizer(L2), and Normalizer(Max).

The best way to make an analysis of these three algorithms was by defining many functions, using for loops to obtain various dataframes that connect our clusters to the number of principal components of our desire, and finally plotting them alongside one another. 

We also added a classification report that shows the performance of these algorithms in terms of `precision`, `recall`, `accuracy`, `f1_score`, etc.

When it comes to selecting principal components, usually we assume that the first 2 principal components explain at least 80 percent of the variance but based on the graphs you see, that is not the case. 

Using the forest fires dataset, we decided to cluster the data by month but obviously clustering by 12 groups is a lot. If we decide to cluster with that many groups, expect to see many outliers and a chance of overfitting. So, we divided the 12 months into three different periods, so January to April would be one period and so on. 

We will break down and compare each algorithm by use of PCA and analyze the classification report of each scaler.

KMeans:

- MinMaxScalar produces highest accuracy with PCA
- `Precision`, `Recall`, and `F1 Score` are highest using the MinMaxScaler and Normalizer(L2) with PCA
- Expect to see that certain scalers will have the same values

Agglomerative:

- It’s quite strange to see that all scalars have the exact same values
- Normalizer(L1) performs at the highest accuracy with or without PCA
- Does a top down approach cause PCA to not make a difference?

Spectral:

- Spectral Clustering seems to perform with similar accuracy and results with or without the use of PCA
- Normalizer(Max) produces the highest `precision` and `f1_score` despite the accuracy having a value a little over a half


# Reflection Questions - Justin
**What do I believe I did well on this assignment?**  
I did well on using the for loop to make the classification reports and plots.

**What was the most challenging part of this assignment?**  
The most challenging part was analyzing the differences between the clustering algorithms in terms of PCA and the different scalars.

**What would have made this assignment a better experience?**  
If there was more than one function to find the optimal number of clusters, that would have helped.

**What do I need help with?**  
I would need help understanding why the agglomerative cluster has no changes in the classification report with or without using PCA.


# Reflection Questions - Daniel
**What do I believe I did well on this assignment?**   

**What was the most challenging part of this assignment?**  

**What would have made this assignment a better experience?**  

**What do I need help with?**   


# Reflection Questions - Ryan
**What do I believe I did well on this assignment?**  

**What was the most challenging part of this assignment?**  

**What would have made this assignment a better experience?**  

**What do I need help with?**  


## License

The license to be used is [MIT](https://choosealicense.com/licenses/mit/)