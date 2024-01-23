# WORK
import matplotlib.pyplot as plt
import pandas as pd
from sklearn.cluster import KMeans
wainaina = pd.read_csv(r'/content/Mall_Customers.csv')
# Specify the optimal number of clusters
optimal_clusters = 5
# User-defined attributes to visualize (you can modify this)
attributes_to_visualize = ['Annual Income (k$)', 'Spending Score (1-100)']
# Select the data for visualization based on user-defined attributes
X = wainaina[attributes_to_visualize].values
…c='red', label='Centroids')
# Move the legend outside
plt.legend(loc='upper left', bbox_to_anchor=(1.01, 1))
plt.title('K-Means Clustering')
plt.xlabel(attributes_to_visualize[0]) # Set X-axis label
plt.ylabel(attributes_to_visualize[1]) # Set Y-axis label
plt.show()
