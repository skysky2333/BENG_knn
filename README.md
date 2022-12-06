# Machine learning - KNN




# K-neighbors classification
KNN is a simple yet effective machine learning classification approaches. This section will explain the details behind K neariest neighbors algorithm.

## Intuition
> You are who you surround yourself with.
> -- <cite>Jennifer Fedinec</cite>
> 
This is the idea behind KNN algorithm. In the N-dimentional database, given a new datapoints, the KNN will looks at its neighbor to determine its classification. For example, if the majority of its neighbors belongs to class A, the new datapoint will be classified as class A.

To define the size of neighbor, a parameter K will be set beforehand. A larger K will considers more neighbor, while a smaller K will consider less / closer neighbors.

## Implementation
To dive deep into its implementation, let's consider a case where a unknown sample need to be classified in a 2-D plane.

<img src="img/Screen%20Shot%202022-12-05%20at%205.46.23%20PM.png" width="500">

<cite>From https://www.ibm.com/topics/knn</cite>

Here, we see neighbors of both classes surrounding the new example. Let's first define the K for the algorithm to start working.

1. Take in user input to define the parameter k to be 3.

Next, the model will look at the 3 nearest neighbor.

2. The model checks out the 3 neighbors, and get 1 class A and 2 class B data points.

<img src="img/Screen Shot 2022-12-05 at 5.59.17 PM.png" width="500">

After getting these data, the model will classify the new datapoint to be the majory class of its neighbors.

3. Because there are more class B than class A neighbors, the new datapoints is classified as class B.


## Distance metrics
On a higher dimentional space which is common in bioinformatic application, difference distance metrics will lead to different results and have their own advantages as well as disadvantages. Let's discuss the two most common distance measurments.

* Euclidean Distance

  The Euclidean distance measure distance in Euclidean space based on Pythagoras' theorem. It is calculated by taking the square root of the sum of the squared pair-wise distances on all dimensions.
  
  <img src="img/Screen Shot 2022-12-05 at 6.15.55 PM.png" width="300">
  
  > \sqrt{\sum_{i=1}^n (x_i-y_i)^2}

* Manhattan distances
  
  Instead of calculating the shortest direct path between two points, Manhattan distance calculates the distance based on gridlines.

  <img src="img/Screen Shot 2022-12-05 at 6.16.02 PM.png" width="300">

  > \left(\sum_{i=1}^n |x_i-y_i|^p\right)^{1/p}

Both metrics are intuitive and fast to compute, therefore widely used in KNN applications.


## Normalization
Because large values in some dimentions will overpower and skew the algorithm to ignore dimentions of smaller values, which may inclose important informations, we need a way to standardize all datapoints across all dimentions. This is where normalization comes in.

One simple normalization stratigy is to rescale all features within range 0-1.

## Importance of K
The only and most curcial hyperparameter to tune for KNN is k.

<img src="img/Screen Shot 2022-12-05 at 6.27.31 PM.png" width="1000">

A small k will overfit and model and create inaccurate bondaries. A large k will under fit the model and create overly-generalized bondaries. So a common stragies is to try multiple iteration of k and choose the best performing one. This is possible because of the low computational cost of KNN.