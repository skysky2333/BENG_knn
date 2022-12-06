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


