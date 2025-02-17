# MNIST-Classification

***Overview***:
This repository contains IPython Notebook for classifying handwritten digits using the MNIST dataset. The notebook demonstrates how to download the data(fetch_openml()), spit the test set and the training set, and finally how to train different classifiers and choose the best algorithm based on not only accuracy but also precision, recall, and f1 score(the harmonic mean of precision and recall).

***Dataset***:
Scikit-Learn provides many helper functions to download popular datasets. The following code fetches the dataset from OpenML.org

from sklearn.datasets import fetch_openml
mnist = fetch_openml('mnist_784', as_frame = False)

***Classifiers used and tested***: SGD(Stochastic Gradient Decent) Classifier, Support vector machines(SVC), OneVsRest(OvR), Random Forest Classifier, and finally K-Nearest Neighbors(KNN).

***Best model**: It was observed that KNN performed pretty well than the others, with an f1 score of 0.9672164755274893

