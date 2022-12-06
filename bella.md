## Clustering v.s. Classification
---
Classification and Clustering are two common machine learning methods to categorize objects into different classes based on features. Classification deals with identifying which new categories does this new object belongs to, on the basis of known labels in a training set of data. 

<br>

For instance, suppose we want to predict whether a student will get an A in BENG183 based on its first 3 homework grades (features). This is a binary classification problem since the outcomes will be:

1. Student gets an A, a result labeled “True”
2. Student does not get an A, a result labeled “False”.

In summary, classification requires a set of observations (training data) which comprises actual classification results (labels). We train the model, called Classifier on this dataset, and use that model to predict whether a student will get an A in BENG183 or not. 

<br>

![Image](https://media.geeksforgeeks.org/wp-content/uploads/classification-1.png)
<cite>From https://www.geeksforgeeks.org/getting-started-with-classification/</cite>
<br>

Clustering deals with dividing the population into subpopulations such that data points in the same groups are more similar within data points in the same group and different between data points in other groups. Clustering does not require any label in the training set so it’s also an unsupervised learning method.


<br>

![Image](https://media.geeksforgeeks.org/wp-content/uploads/clusteringg.jpg)
<cite>From https://www.geeksforgeeks.org/clustering-in-machine-learning/</cite>

<br>

For instance, if we want to discover whether a newly discovered specie falls into category A or category B, clustering would be a great method to use.

<br>

![Image](https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/Phylogenetic_tree.svg/900px-Phylogenetic_tree.svg.png)
<cite>From https://en.wikipedia.org/wiki/Phylogenetic_tree</cite>

<br>

More difference between classification and clustering can be found in this table:

|Classification| Clustering |
|:----------------:|:----------------:|
|Uses labelled data as input    |Uses unlabelled data as input|
|Training and testing sets needed| Training and testing sets not needed|
|Supervised learning| Unsupervised learning|
|More complex| Less complex|
|Examples algorithms: Logistic regression, Naive Bayes classifier, Support vector machines, etc.|Examples algorithms: k-means clustering algorithm, Fuzzy c-means clustering algorithm, Gaussian (EM) clustering algorithm, etc.|

---

<br>

## Summary


Machine learning algorithms in bioinformatics can be used for prediction, classification, and feature selection. Machine learning has many applications such as in biology and bioinformatics. For instance, Artificial neural networks in bioinformatics have been used for:

* Comparing and aligning RNA, protein, and DNA sequences.
* Identification of promoters and finding genes from sequences related to DNA.
* Interpreting the expression-gene and micro-array data.
* Identifying the network (regulatory) of genes.
* Learning evolutionary relationships by constructing phylogenetic trees.

Prior to the rise of machine learning, bioinformatics calculations had to be done by hand, and this bring difficulty for issues such as protein structure forecasting. Machine learning has already greatly benefited the study of bioinformatics. In the future, we believe that with the advancement of machine learning, bioinformatics will be able to solve more complex biological and public health related problems.



