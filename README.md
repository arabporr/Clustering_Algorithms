# Comparing different clustering algorithms on three datasets
## Introduction
This project was part of my Data Mining course, in which we were given three datasets, and we should try some different clustering methods on them.

## Methodology
First off, I loaded the data in Colab. Then, I normalized the datasets and plotted them to gain some insights:
```

```

After that, I found the elbow point for the number of clusters:
```
```

Then, I tried different algorithms and ended up with the following results:
```
```

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
