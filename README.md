# Recommendation with Collaborative Filtering-ALS

# Movie recommendations for users
## TABLE OF CONTENTS

* [Objective](#objective)
* [Data](#data)
* [Libraries and versions](#Libraries and versions)
* [Technologies](#technologies)
* [Algorithms](#Algorithm)
* [Implementation](#implementation)
* [Results](#results)

## OBJECTIVE
The main objective of the project is to design a movie-recommendation engine for the users.

## DATA
one data sources were referred.

1. [Movielens data : Consisting of 1502 inctances of movie ratings provided by users.



## LIBRARIES AND VERSIONS
python 3.8.10
numpy 1.22.3
ubuntu Desktop 20.04.4
findspark 2.0.1
spark 3.2.1


## TECHNOLOGIES
virtualbox and ubuntu to use pyspark
Python - Spark, pyspark, numpy, findspark 

## ALGORITHMS
- Collaborative Filtering using ALS algorithm

## IMPLEMENTATION
### Collaborative filtering -ALS algorithm:
Collaborative filtering technique allows filtering out items that a user might like by leveraging
the ratings of similar users. The underlying assumption in recommendation using collaborative
filtering is that, if the user A and user B share a similar response (movie rating in our case) to a
movie, then they are likely to share a similar response to any movie X, compared to any random
user.

- Employed the model-based system of performing collaborative filtering on the MovieLens dataset. 
- Implemented Alternating Least Square(ALS) with Spark. ALS is a matrix factorization technique to perform collaborative filtering. The
objective function of ALS uses L1 regularization and optimizes the loss functions using Gradient Descent. 
- The dataset contained movieId and ratings in the format of a user-rating matrix. 


 I train the ALS model by tuning the below hyper-parameters:
maxIter: The maximum number of iterations the algorithm is run
regParam:The L1-regularization parameter used in ALS algorithm


After tuning the parameters and implementing ALS with Cross validation an optimal RMSE value of 1.0534 at the regParam value of 0.5 in 10 iterations.

Below are the resulting movie predictions made by the tuned ALS model on the test data 

![image](https://user-images.githubusercontent.com/80451122/162593191-c0a98979-8425-43a4-8186-4452b2c22bdb.png)

Refer to this link for code: https://github.com/reyhandagcigsu/Recommendation-with-Collaborative-Filtering---ALS/blob/main/ALS%20with%20movielens-small.ipynb


## RESULTS
The movie recommendation system has shown tremendous potential. Movie recommendations have been pretty accurate for specific users


