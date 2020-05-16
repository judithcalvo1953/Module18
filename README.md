# Module18
This project explores a dataset of bitcoins to determine the major clusterings, using unsupervised machine learning, which, in contrast to supervised machine learning, there is no designated outcome variable that we are trying to predict.  We are simply aiming to see which of the bitcoins tend to be more similar than others.  We use two methods in this module: PCA and K-Means Clustering.

## PCA (Principal Components Analysis)
This exercise used 3 components.  The resulting explained variance for each of the three components were: PC1-2%, PC2-2% and PC3-2%.  This leads me to conclude that this method did not find any predominant components that could explain variance in bitcoin typology.  Much unexplained variance remains in the bitcoin values that cannot be explained by the PCs.  Nevertheless, looking at the loadings of each bitcoin type in the DataFrame of the loadings, we can see that PC2 seems to load more heavilty on many of the bitcoins shown.  By contrast, others load heavily on PC2 in the opposite direction, with negative loadings.  Loadings are the proportion of each bitcoin value on an axis that contributes to the Principal Components (my interpretation derived from video viewed on 5/16/20-- https://www.youtube.com/watch?v=FgakZw6K1QQ, PCA step by step by Josh Starmer).  This is noisy data, with much not accounted for with the PCA approach

Not really possessing a solid knowledge of bitcoins, as I might have knowledge, of say, items that purport to measure some psychological state, such as depression or anxiety, I don't find the PCA analysis to be very informative in understanding bitcoin "behavior".  Now let's look at the K-Means.

## K-Means Clustering

The K-Means Clustering is a bit ("pardon the pun") more informative.  One can see that there is one outlier (BitTorrent) that does not fit into any of the 3 clusters shown in the 3-D graph.  Class 1 aligns more with PC2. The few bitcoins in class 3 load heavily on PC3, and finally Class 0 loads more on PC 1.

## Conclusions
I don't derive any solid conclusions from this data. I suppose that if I were to invest in bitcoins, I'd be more likely to research those belonging to Class 0 and Class 1, in order to find other features that might explain why they cluster.  The given data seems too sparse to understand bitcoin action, given that the three PCA's we used only explained 6% of the variance in bitcoin categories.
