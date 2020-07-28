# News Articles Text Classification and Clustering

In this repository we perform **Text Classification** and **Clustering** experiments. 
Also, generating **Word Clouds for each article category**.

The **input consists of 2225 documents** from a news site that corresponds to stories in five local areas 
from 2004-2005.

**Document Categories**
* Business
* Entertainment
* Politics
* Sport
* Tech

First line of each document is the title and the rest is the content of the article.

The **whole procedure** consists of:

1) **Create a data set of all documents**
2) **Text pre-processing**
   1) Remove special characters, lower case
   2) Remove Stopwords
   3) Lemmatization
   4) Stemming
   5) Tokenization
3) **Generate Word Clouds**
4) **Vectorization**
5) **Classification** and **Clustering**

I also implemented a KNN Classifier using max heap, but it was **too slow** for this data set.

## Word Clouds

<h2 align="center"> Business </h2>

![business](https://user-images.githubusercontent.com/48658768/90988571-6166b000-e59c-11ea-99ce-163762bb3b5e.png)

<h2 align="center"> Entertainment </h2>

![entertainment](https://user-images.githubusercontent.com/48658768/90988567-5d3a9280-e59c-11ea-922d-5982b57de1d0.png)

<h2 align="center"> Politics </h2>

![politics](https://user-images.githubusercontent.com/48658768/90988568-5e6bbf80-e59c-11ea-8cd2-998e29bdcef4.png)

<h2 align="center"> Sport </h2>

![sport](https://user-images.githubusercontent.com/48658768/90988569-5f9cec80-e59c-11ea-93a9-3957d0b4b9cb.png)

<h2 align="center"> Tech </h2>

![tech](https://user-images.githubusercontent.com/48658768/90988570-60358300-e59c-11ea-9871-097476f73eac.png)

## Classification

Classifier: MultinomialNB, SVM, RF, KNN

Vectorization: Bag Of Words, Tf-idf

Dimensionality Reduction: PCA, SVD and ICA

### Roc curves

![multinomialnb_bow_roc_curves](https://user-images.githubusercontent.com/48658768/90987463-d97ca800-e593-11ea-8089-949a30320437.png)

![multinomialnb_tf_idf_roc_curves](https://user-images.githubusercontent.com/48658768/90987464-da153e80-e593-11ea-909d-164624f3d1e8.png)

![svm_bow_roc_curves](https://user-images.githubusercontent.com/48658768/90987468-daadd500-e593-11ea-8128-756ee918aa29.png)

![svm_tf_idf_roc_curves](https://user-images.githubusercontent.com/48658768/90987469-db466b80-e593-11ea-8971-798d4cc917e7.png)

![random_forest_bow_roc_curves](https://user-images.githubusercontent.com/48658768/90987465-da153e80-e593-11ea-93a4-3e1b46599197.png)

![random_forest_tf_idf_roc_curves](https://user-images.githubusercontent.com/48658768/90987467-daadd500-e593-11ea-86cf-d6d6c31adce9.png)

![knn_bow_roc_curves](https://user-images.githubusercontent.com/48658768/90987470-db466b80-e593-11ea-93c3-ecead0cbc5f3.png)

![knn_tf_idf_roc_curves](https://user-images.githubusercontent.com/48658768/90987471-dbdf0200-e593-11ea-9988-7d66cbdb2eb4.png)

### 

## Clustering

Clusterer: Kmeans

Vectorization: Bag Of Words, Tf-idf, Word2vec

Dimensionality Reduction: PCA, SVD and ICA

<h2 align="center"> PCA </h2>

![bow_pca](https://user-images.githubusercontent.com/48658768/90987319-b6052d80-e592-11ea-8fe6-49b92914a284.png)

![tf_idf_pca](https://user-images.githubusercontent.com/48658768/90987322-b7cef100-e592-11ea-912a-5e68ca6c2a7e.png)

![word2vec_pca](https://user-images.githubusercontent.com/48658768/90987325-b9001e00-e592-11ea-9a85-d959e52668f3.png)

<h2 align="center"> SVD </h2>

![bow_svd](https://user-images.githubusercontent.com/48658768/90987320-b7365a80-e592-11ea-9340-1db8ca452ac5.png)

![tf_idf_svd](https://user-images.githubusercontent.com/48658768/90987323-b7cef100-e592-11ea-84e1-cd0086a1c2b9.png)

![word2vec_svd](https://user-images.githubusercontent.com/48658768/90987326-b9001e00-e592-11ea-99d2-3547509550a8.png)

<h2 align="center"> ICA </h2>

![bow_ica](https://user-images.githubusercontent.com/48658768/90987328-b998b480-e592-11ea-8b01-c858bf3e1d83.png)

![tf_idf_ica](https://user-images.githubusercontent.com/48658768/90987321-b7365a80-e592-11ea-8a9a-6a2f22428970.png)

![word2vec_ica](https://user-images.githubusercontent.com/48658768/90987324-b8678780-e592-11ea-8029-1b86b9ba202d.png)