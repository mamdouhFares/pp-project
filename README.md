# pp-project

K-Means Clustering with Multi-Threading 

# Project Overview
This project implements the K-Means Clustering algorithm using multi-threading in Java. Instead of processing all data sequentially, we use multiple threads to assign points to clusters in parallel, significantly improving performance when working with large datasets.

# steps
1 Reading Data from a Large File (data.csv)

The program reads a large dataset from a CSV file containing X, Y coordinates.
2 Dividing Data Among Multiple Threads

The dataset is split into equal parts, and each thread processes a portion of the data simultaneously.
3 Assigning Points to the Nearest Cluster in Parallel

Each thread calculates the distance between its assigned points and the cluster centroids, then assigns them to the nearest cluster.
4 Waiting for All Threads to Finish

The main program waits for all threads to complete before updating cluster centroids.
5 Repeating Until Clusters Stabilize

The process repeats until cluster centroids do not change significantly, ensuring an optimal clustering result.

# Final Output
The program prints the number of iterations required to reach stable clusters
