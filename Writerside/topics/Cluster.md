# Cluster

In statistics, clustering is a technique used to group similar data points into clusters or groups based on certain criteria. 

>The goal of clustering is to identify patterns or structures within a dataset by grouping data points that are similar to each other than to those in other clusters. 

There are various clustering algorithms, each with its own approach to defining similarity and forming clusters. 

__BioStat Prime comes up with a platform to perform the algorithms to aid users in their analysis.__

### Hierarchical Clustering

This sub menu provides Hierarchical cluster analysis on a set of dissimilarities and methods for analyzing it.

Hierarchical clustering builds a hierarchy of clusters, creating a tree-like structure (dendrogram) that shows the relationships between clusters at different levels.

To analyse it in BioStat Prime user must follow the steps as given.

Steps
: __Load the dataset -> Click on the analysis tab in main menu -> Select CLUSTER button -> Select Hierarchical Cluster -> This leads to the analysis technique in the dialog -> Select the source variable -> Write no. of clusters values -> Execute the dialog.__

The result of the analysis will be visible in the output. Users can also decide whether to __assign cluster values to dataset__, __plot cluster dendrogram__, __show cluster bi plot__. 

The options tab at the bottom leads the user to further methods and metrics that the user can choose according to the requirements.

![Hierarchical Clustering](screenshots/Hierarchical Clustering.png){ width="700" }{ border-effect="rounded" }

> Arguments
>1. __varsToCluster__: The variables to analyze
>2. __method__: the agglomeration method to be used. This should be (an unambiguous abbreviation of) one of "ward.D", "ward.D2", "single", "complete", "average" (= UPGMA), "mcquitty" (= WPGMA),"median" (= WPGMC) or "centroid" (= UPGMC).
>3. __noOfClusters__: The number of clusters desired
>4. __plotDendogram__: Plot a dendogram True or false
>5. __assignClusterToDataset__: Save the cluster assignments to the dataset
>6. __label__: name for the new variable that stores the cluster assignments
>7. __plotBiplot__: plot Biplot TRUE or FALSE

### K-Means Clustering

This sub menu performs K-means clustering.

K-Means is a popular partition clustering algorithm that aims to partition data into K clusters. It iteratively assigns data points to clusters and updates cluster centroids until convergence. 

>Partition clustering divides the data into non-overlapping clusters in a single step.

To analyse it in BioStat Prime user must follow the steps as given.

Steps
: __Load the dataset -> Click on the analysis tab in main menu -> Select CLUSTER button -> Select K-Means Cluster -> This leads to the analysis technique in the dialog -> Select the source variable -> Write no. of clusters values -> Execute the dialog.__

The result of the analysis will be visible in the output. User can also decide whether to `assign cluster values to dataset`, `show cluster bi plot`, `no. of starting seeds`, `maximum iterations`.

![K-Means Clustering](screenshots/K-Means Clustering.png){ width="700" }{ border-effect="rounded" }

>Arguments
>1. __vars__: The variables to analyze in a vector of form c('var1','var2'...)
>2. __centers__:either the number of clusters, say k, or a set of initial (distinct) cluster centers. If a number, a random set of (distinct) rows in x is chosen as the initial centers.
>3. __iter.max__: the maximum number of iterations allowed.
>4. __num.seeds__: The number of different starting random seeds to use. Each random seed results in a different k-means solution.
>5. __storeClusterInDataset__ : Save the cluster assignments to the dataset
>6. __varNameForCluster__: The variable names for the assigned clusters
>7. __dataset__: The dataset to analyze