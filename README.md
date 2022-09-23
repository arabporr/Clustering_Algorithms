# Comparing different clustering algorithms on three datasets
## Introduction
This project was part of my Data Mining course, in which we were given three datasets, and we should try some different clustering methods on them.

## Methodology
First off, I loaded the data in Colab. Then, I normalized the datasets and plotted them to gain some insights:

![First_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/First_Dataset.png)

![Second_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/Second_Dataset.png),

![Third_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/Third_Dataset.png)


After that, I found the elbow point for the number of clusters:

![Elbow_Curve_First_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/Elbow_Curve_First_Dataset.png)

![Elbow_Curve_Second_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/Elbow_Curve_Second_Dataset.png),

![Elbow_Curve_Third_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/Elbow_Curve_Third_Dataset.png)


Then, I tried different algorithms and ended up with the following results.

## Results
### First Dataset:
![K-means_First_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/K-means_First_Dataset.png)

![Fuzzy_C-means_First_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/Fuzzy_C-means_First_Dataset.png),

![DBScan_First_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/DBScan_First_Dataset.png)

### Second Dataset:
![K-means_Second_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/K-means_Second_Dataset.png)

![Fuzzy_C-means_Second_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/Fuzzy_C-means_Second_Dataset.png),

![DBScan_Second_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/DBScan_Second_Dataset.png)

### Third Dataset:
![K-means_Third_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/K-means_Third_Dataset.png)

![Fuzzy_C-means_Third_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/Fuzzy_C-means_Third_Dataset.png),

![DBScan_Third_Dataset](https://github.com/arabporr/Clustering_Algorithms/blob/7b8299f117755e379ef929c69a9722f3f58509df/Plots_Images/DBScan_Third_Dataset.png)

## Conclusion 
From what we saw from different algorithms, the density-based models are good when the data are inherently separated locally; so the algorithm worked quite well in the second dataset but not that well in the other two (based on the SSE error measure.)

The K-means and the Fuzzy C-means both worked well, and in comparison to each other, the K-means was a little bit better, to be honest.

So, to sum up, Models by their total performance:
- K-means
- Fuzzy C-means
- Density Based (DBScan)

Models by their usage:
- for common data: K-means
- complex and not separated data: Fuzzy C-means
- spacial complex but well-separated: Density Based
