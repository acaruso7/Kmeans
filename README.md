# Kmeans
An implementation of Kmeans clustering using only Python data structures (lists, tuples, dicts)

This simple implementation of Kmeans takes a list of two dimensional tuples as input, along with the desired number of
clusters k and the desired number of model iterations. The algorithm is sensitive to the locations of the initial
centroids (randomly selected), and as such should be run a few times to avoid getting stuck on local minima. The version
with the highest ratio of between-cluster-variance to within-cluster-variance (BCV / WCV) should be selected. This value 
should increase on every iteration.

The number of model iterations should be selected such that the BCV / WCV ratio reaches convergence (no change on every 
next iteration).
