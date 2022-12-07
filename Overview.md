# Overview 💻

<p align="center" width="100%">
<img src="https://user-images.githubusercontent.com/97704603/205791858-a5bfc0ca-7473-4f0a-ab87-6ee47877c7ae.png" width=70% height=70%>
<p>
  
###### Image Source Video https://www.youtube.com/watch?v=ukzFI9rgwfU&t=6s

As humans, we learn from our past experiences and thus could better adjust our performances in the future. 
The first time you have a dinner in a new restaurant, the experience you had in the restaurant would 
influence whether or not you will choose the restaurant again. 
For machines, they are developed and given instructions by humans to help perform some tasks. 
Calculators can be used to help us figure out the square root of an extremely large number. 
For simple tasks like calculating the square root of a number, humans can explicitly program the command. 
However, for advanced tasks, it may be hard for humans to efficiently create the needed algorithms to be put in the machines. 

> ### Machine learning is a method of data analysis that automates analytical model building.  

Here is when **machine learning** comes in handy. **Tasks can be performed by machine learning programs without being explicitly programmed to do. 
Machines learn from the data provided** (Wink-wink, we will talk about details of different datasets later in this chapter) and then perform certain tasks. 
**In Bioinformatics**, application of machine learning algorithms include **genomics, proteomics, microarrays, systems biology, evolution, and text 
mining**.
  
<p align="center" width="100%">
<img src="https://user-images.githubusercontent.com/97704603/205791233-9f680b86-0e11-4644-8e39-b919d1d7e785.png" width=70% height=70%>
<p>
  
###### Image generated from https://monkeylearn.com/word-cloud/

## Simple kNN Application Example in Bioinformatics
We created animation video we created to simply illustrate how we can implement kNN algorithm to classify Diabetic Patient given age and BMI =)
<p align="center" width="100%"><img width="680" alt="Screen Shot 2022-12-06 at 5 04 40 PM" src="https://user-images.githubusercontent.com/97704603/206062418-ad414215-c374-4811-b945-fa29100c191f.png"><p>


[Click me to watch videos👉👈](https://youtu.be/5nogFDZDz_k)

<p align="center">
<img width="660" alt="1" src="https://user-images.githubusercontent.com/97704603/206064649-162bd391-fd11-41b2-bc8e-b38c6694241d.png">
<p>
As you may learn in the following sections, for supervised learning algorithm (classification), we need to have a training dataset before we want to classify the new datapoint. Here is a group of people that we will record their BMI and ages for training dataset generation. (SUPER SIMPLE DATASET)

<p align="center">
<img width="660" alt="2" src="https://user-images.githubusercontent.com/97704603/206064653-d18740b9-0895-49f8-805a-831f1e386d53.png">
<p>
Healthy patients will be marked as pink points on the graph, while diabetic patients will be marked as yellow points.  

<p align="center">
<img width="660" alt="3" src="https://user-images.githubusercontent.com/97704603/206064656-3380a833-f5f4-4feb-81af-02e470ae5e18.png">
<p>
After the machine is given the training dataset, it will be given a new data point, which is needed to be classified. Here, the new data point is a middle-age male with BMI in overweight range.
  
<p align="center">
  <img width="660" alt="4" src="https://user-images.githubusercontent.com/97704603/206064659-cb1effe9-f98b-400a-911d-fbac4630969d.png">
<p>
kNN algorithms(k Nearest Neighbors Algorithm) can be implemented to classify this new data point. k is a user-defined number of neighbors.
We will talk about how to choose k and what kNN algotithm is in our following section.

<p align="center"> 
  <img width="660" alt="6" src="https://user-images.githubusercontent.com/97704603/206064660-1f62aa34-0001-4662-a23d-0d5aaf45690e.png">
<p>
After choosing the k and check the number of neighbors in different groups, this new data point can be classified to diabetes group as it has more yellow point neighbors.

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
###### From https://www.geeksforgeeks.org/getting-started-with-classification/
<br>

Clustering deals with dividing the population into subpopulations such that data points in the same groups are more similar within data points in the same group and different between data points in other groups. Clustering does not require any label in the training set so it’s also an unsupervised learning method.


<br>

<p align="center">
<img width="680" alt="2" src="https://media.geeksforgeeks.org/wp-content/uploads/clusteringg.jpg">
<p>
  
###### From https://www.geeksforgeeks.org/clustering-in-machine-learning/

<br>

For instance, if we want to discover whether a newly discovered specie falls into category A or category B, clustering would be a great method to use.

<br>

<p align="center">
<img width="680" alt="2" src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/Phylogenetic_tree.svg/900px-Phylogenetic_tree.svg.png">
<p>
  
###### From https://en.wikipedia.org/wiki/Phylogenetic_tree

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




  

