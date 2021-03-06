# Recommender-System
In this project, I attempted to construct a recommendation system to promote users with new movies that are likely to match their tastes. The two methods discussed in this project are first, matrix factorization, and secondly, ensemble modeling on top of matrix factorization. In other words, with ensemble modeling, the predicted results from matrix factorization become one of the features for the second stage model. I discovered that the ensemble approach is able to decrease the mean absolute error (MAE) of our predictions by a noticeable margin compared the naive matrix factorization approach. 

One major challenge that I faced throughout the experimentation is that given a large dataset, both our matrix factorization algorithm and second stage machine learning models require a long time to execute. Therefore, future work can be focused on running the models with better computation resources, for example, on GPU.

## Data
The dataset for this project comes from the MovieLens website by GroupLens Research. Since we do not have access to more computation resources, we choose the smaller dataset version that contains 100,836 ratings across 9,742 movies. These data were created by 610 users between March 29th, 1996 and September 24th, 2018. Each rating ranges from 0.5 stars to 5 stars with an increment of half stars. In addition, we further reduce the scope of the dataset by dropping all movies with less than 20 ratings. As a result, the modified dataset contains 67,898 ratings across 1,297 movies created by 610 users. In this dataset, each user and movie is represented by a unique ID, which can be used to join with other tables, such as a movie table that contains the information about movie titles and genres.

The link to access the dataset is: https://grouplens.org/datasets/movielens/

## Technical Details and Results
Please see "Project Report" for more technical details and project results.
