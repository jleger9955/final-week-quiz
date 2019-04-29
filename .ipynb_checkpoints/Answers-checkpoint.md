# Data Science Quiz

### Instructions

- Fork and Clone
- Work on quiz
- Push back up to your repository

### Questions

1. A vector is given, `[2,3,9]`. What's the norm?
   9.695 
2. I have a biased 6-sided die. P(T) = 0.45. What's the probability, if I flip the coin 100 times, that I will get exactly 14 heads?
   1.5369077164427643e-17 (nearly zero)
   scs.binom(100, .55).pmf(14)
3. What is the rank of a matrix?
   The number of linearly independant rows/columns
4. Why is rank important for Linear Regression?
   Linear regression involves inverting the feature matrix. The matrix must be full-rank in order to be inverted. 
5. What is the purpose of the sigmoid function in a Logistic Regression model?
   The sigmoid function converts the log odds into probabilities.
6. What is bias vs variance?
   High bias leads to under-fitting. High variance leads to over-fitting.
7. What is a hyperparameter? What part of the dataset (train, validation or test) is responsible for determining this value?
   A hyperparamter is any parameter in our model that can be tuned to make our model more accurate. The validation data.
8. Model selection via cross validation. What part of the dataset (train, validation or test) is responsible for choosing the best model?
   Test data
9. What is parametric vs non-parametric model?
   A parametric model involves the learning of certain parameters based on the train data set. A non-parametric model has no learned parameters. 
10. What models do you need to scale the data prior to fitting?
    Parametric models typically require us to scale the data.
11. What is entropy? Which model uses this concept?
    Entropy is a measure of diversity/disorder. It is used in Decision Trees and Random Forest models to calculate Information Gain. 
12. How is a random forest generated?
    A Random Forest model involves bagging the data and randomly selecting features to create several different Decision Trees. A majority vote of all the trees in the forest is then used to make a prediction.
13. How do you determine the correct number of clusters when using KMeans?
    The elbow method which involves plotting the within-cluster sum-of-squares for each cluster and finding the 'elbow'. You could also plot the Silhouette score for each cluster.  
14. What is a dendrogram?
    A plot of the linkage matrix that gives us a visual representation of the hierarchical clusters.
15. What is linkage?
    The linkage function is used to generate hierarchical clusters by measuring the distance between each cluster (in variace ways). The linkage matrix is used as the input to create the dendrogram
16. How does a recommender model work?
    It uses Non-Negative Matrix Factorization(NMF) to identify the "hidden features" in a matrix.
17. How can you reduce the number of features in a model?
    a. Use Lasso to identify which features to keep
    b. Review the correlation matrix to identify the most relevant features
    c. You could get the feature importance from a decision tree model
    d. Use PCA to compress multiple features
18. What is a good use of PCA?
    Plotting high dimensial data on a 2 or 3 dimensional plot
19. In general, how do neural networks "learn"?
    They learn by optimizing the loss function to determine the new bias and weights for each feature (back propagation) during every iteration of the process. 
20. What is your favorite model? Why?
    Gradient Boosted Decision trees. They are flexible(can be used for either Regression or Classification) and seem to out perform most other models. They are also much easier to train than Neural Networks. 