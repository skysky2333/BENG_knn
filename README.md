# Machine learning - KNN




# K-neighbors classification
KNN is a simple yet effective machine learning classification approaches. This section will explain the details behind K neariest neighbors algorithm.

## Intuition
> You are who you surround yourself with. --- Jennifer Fedinec

This is the idea behind KNN algorithm. In the N-dimentional database, given a new datapoints, the KNN will looks at its neighbor to determine its classification. For example, if the majority of its neighbors belongs to class A, the new datapoint will be classified as class A.

To define the size of neighbor, a parameter K will be set beforehand. A larger K will considers more neighbor, while a smaller K will consider less / closer neighbors.

## Implementation
To dive deep into its implementation, let's consider a case where a unknown sample need to be classified in a 2-D plane.
<img src="img/Screen%20Shot%202022-12-05%20at%205.46.23%20PM.png" width="500">

