# Adaptive K-means clustering  
https://www.aaai.org/Papers/FLAIRS/2004/Flairs04-119.pdf  

Two techniques suggested by the paper  
. Algorithm for Adaptive K-Means Clustering  
. Threshold-Based Clustering Algorithm


Algorithm for Adaptive K-Means Clustering
---
Three cases
let distance between two closest clusters(c1 ans c2) = dmin
    distance of element to its neraest cluster = d
1. if d of new element to nearest cluster is zero, add element to the cluster.
2. if d is lesser than dmin, add to nearest cluster. Centroid of this cluster would change. Recalculate it.
3. if d is greater than dmin, merge c1 and c2 and create new cluster with new element.

Threshold based clustering algorithm
---
if less than threshold, add element to cluster.
if recomputed distance between two clusters is less than a threshold, merge the clusters.


### Image segmentation using adaptive k-mean
https://link.springer.com/content/pdf/10.1186/s13640-018-0309-3.pdf  
Method
===
1. Image preprocessing  
1. 1. Image normalization  
1. 1. 1. Size of image is normalized, so that subsequent segmentation can be carried out quickly.  
1. 2. L*a*b* color space conversion (RGB–to-XYZ-to–L*a*b*)
1. 2. 1. the beauty of the L*a*b* color model is that it compensates for the inequality of the color distribution of the RGB color
1. 2. 2. we found that different food images will inevitably cause uneven background due to differences in conditions such as light and the color of the food itself, which will seriously affect the segmentation results. Therefore, we take the L* component, the luminance component, in L*a*b* as a fixed value x
1. 2. 3. RGB–XYZ–L*a*b*
1. 3. #### Adaptive K-means 

Steps to Implement:  
===
1. Image normalization  
2. Conversion RGB -> XYZ -> L*a*b (formulas given in the paper
3. Fix L* value to x.




## Codes
Opencv-adaptive k mean
===
https://github.com/TommyR22/OpenCv-Adaptive_Kmeans_Clustering
In this code:  
. Intensity is used as measure to group pixels.  
. Threshold is used to create clusters.  
. Threshold is used to murge close clusters.






