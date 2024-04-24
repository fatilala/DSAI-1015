# SC1015 Mini-Project - Song Popularity Prediction
## ABOUT
Our project aims to predict whether a song will be popular amongst the general public based on the song’s features, like loudness, energy, etc.
We utilised data science concepts by importing a spotify dataset and training a model in order to predict a certain trend or outcome and derive information that can help us in making an informed decision. 
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Practical Motivation and Problem Definition
We are simulating playing the role of a record label/music producer who is interested in looking at the performance of artists and how well their songs might perform based on the song’s elements.
While popularity of a song or the capability of a song to rank high on charts may be influenced by the current trends, the various components that make up a song may be the answer for producing a hit song. Therefore, one can then predict how well a newly released song can perform based on these patterns. Therefore, these producers would want to predict how well a song will perform based on different metrics and song characteristics to appeal to a larger audience. 

Hence, our problem definition: 

   Discovering if it’s possible to predict popularity of a song using its features, and in the process, examining other secondary features as well such as which genre is the best          performing genre in terms of popularity.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## ML TECHNIQUES WE USED: 
1) Linear regression
2) Decision tree
3) AdaBoost Classifier
4) K means Clustering
5) Deep FeedForward Neural Network

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## OUR PROJECT FILES:

### 1) EDA Notebook : Data extraction and Exploratory Analysis
  ◦ Read in data from kaggle -> import the CSV file of the spotify tracks
  
  ◦ Explored the different features of the songs to identify the numerical and categorical variables that can be used to predict popularity
  
  ◦ Uni-variate statistics done to observe the features
  
  ◦ Plotting joint plots and correlation matrix of features with the popularity


### 2) Regression & Classification Notebook:

   ◦ LINEAR REGRESSION:
      - We selected certain song features based on the the correlation matrix alongside popularity
      - Performed univariate regression.  
      - Performed multivariate regression with popularity

   ◦ DECISION TREE CLASSIFIER:
      - Converted popularity to a categorical variable and we performed univariate classification.
      - We found a high number of misclassifications hence we used → AdaBoostClassifier which helped reduce misclassifications.
      - Performed multivariate classification utilising the AdaBoostClassifier → we saw better results.


### 3) K Means Clustering Notebook:

   - We sought to tackle the song popularity prediction based on different genres of songs.
   - We grouped the songs into distinct clusters in terms of → many streams, average streams, or less streams.
   - Model then analysed characteristics of songs within each cluster .
   - Our theory was that we could then place a song under one of the clusters based on its features and then predict  popularity of that song.


### 4) Neural Network Notebook:
   
   - Our goal → to use a deep multi-layered neural network, having it take in data from all the 10x features and predict if the song is popular or not. 
   - We opted to use a normal Artificial Feed-forward Neural Network with 5 hidden layers.
   - Employed “MinMaxScaler” alongside to improve accuracy by scaling
   - Input data was split into batch sizes of 128 and run over 30 epochs.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## FINDINGS

  - Popularity didn't seem to have much of a high linear correlation with the features of the songs.
    
  - Found that multivariate models seemed to give better results as compared to univariate.
    
  - Found that our neural network model worked most optimally because of our large dataset and when we utilised more song features.
    
  - Each of the models we used had its own purpose and were optimal in different cases.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## NEW THINGS WE LEARNT:

- AdaBoostclassifier for handling misclassified samples
- Attempting to find clusters within the data
- Importing Keras and Tensorflow for our neural network model
- Applying neural network for prediction
- Clustering using K Means







      




   








   

   

