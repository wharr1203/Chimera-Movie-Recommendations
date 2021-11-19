# Chimera-Movie-Recommendations

## Introduction
Our team, Chimera Solutions, consists of Derek Supino,Jade Adams, and Wayne Harrison. We were tasked with building a reccomendation system on Python for Cinemania's streaming service. The new movie streaming service 'Cinemania' is looking for a way to increase movie streaming by customers. They have asked Chimera Solutions to provide the means of connecting subscribers to movies that they will enjoy, and then link to them to other movies that they will enjoy. The goal of this notebook is to construct a recommendation system that will accurately link subscribers to movies that fit their unique tastes.

## Business Problem
Cinemania is trying to enter the highly saturated streaming service field, and is looking for the means to level the playing field. They need a recommendation system that is accurate enough to give users a reason to use their service over the many other ones.

## Data Exploration
We received 4 datasets, icluding a dataset of ratings on a scale of 1-5.  We investigate the genres with the highest number of reviews and reccommend that Cinemania hones in on hosting movies of this genre on their streaming service so that they can obtain more user data.

## Modeling
We use user reviews of movies to build a user-user collaborative modelling system with the Surprise library. By using grid searches and iterating through the potential algorithms, we were able to find the bst models and paramaters for predicting user ratings and providing movie reccomendations. Our final model is a Singular Value Decomposition algorithm that predicts a users rating of a movie within .64 of their actual rating.

## Final Model Evaluation
 As seen above a model that gives us an MAE of .63 would predict a rating that .63 higher or .63 lower than the true rating given by a user.

## Cold Start Problem
We also investigate how we can provide reccomendations with brand new users with no previous reviews, i.e. the 'cold start solution'. For this situation, we use an item-item correlation scores to provide similar movies. Over time, as users rate movies, we can provide more accurate and diverse reccomendations.

## Conclusion
We were able to create a recommendation model that can predict what a user will rate a movie while only being off by .64 of the true rating on average. We would like to drop our Mean Absolute Error error down to .5, a task that we can definitely get to after obtaining more user data. Having an MAE below .5 would allow us to have confidence in the determined rating.

Please go to the main notebook to see our work as a whole. And comment or email us with any feedback :)
