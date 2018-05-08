## i
5, because the elbow of the graph occurs when K = 5.

## ii
Elbow method is a method to determine the optimum number of cluster to be used in clustering.

To apply Elbow method, we choose a minimum K and a maximum K, (K means number of clusters).  

Then, we train the clusterer (e.g. K-Mean clustering), with each number of K range from the minimum K to the maximum K.  

After that, we calculate the variance for each clusters correspond to the number of K.

At last, we plot it into a graph (Variance against number of clusters), and find the elbow, which is the optimum number of clsuters.