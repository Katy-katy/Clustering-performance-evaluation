# Clustering performance evaluation


Working on image classification app at SLAC I faced a with problem of clustering performance evaluation. Since I have only unlabeled images, I need a metric to evaluate my clusters. I have found that there is two main metrics: Silhouette Coefficient and Calinski-Harabaz Index (http://scikit-learn.org/stable/modules/clustering.html#clustering-performance-evaluation).

According to the documentation, for the both metrics “the score is higher when clusters are  score is higher when clusters are dense and well separated, which relates to a standard concept of a cluster.”

Since it is not very clear from scikit-learn documentation what is the difference between these two metrics, I decided to compare Silhouette Coefficient and Calinski-Harabaz Index.

I have found an example how to use Silhouette Coefficient for selecting the number of clusters (http://scikit-learn.org/stable/auto_examples/cluster/plot_kmeans_silhouette_analysis.html#sphx-glr-auto-examples-cluster-plot-kmeans-silhouette-analysis-py). I decided to extend this example to compare Silhouette Coefficient and Calinski-Harabaz Index. 

Look at this picture - some people could say that there are two clusters, and some could say there are four. Our metrics have the same opinions: Silhouette Coefficient votes for “two” and Calinski-Harabaz  for “four.”

I hope, my visualization makes more clear that when we want to have very well separated clusters, we can use Silhouette Coefficient, and when we want to have more dense clusters, we can use Calinski-Harabaz Index. 
