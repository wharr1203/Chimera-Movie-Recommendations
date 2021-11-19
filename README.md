# Chimera-Movie-Recommendations
Our team, Chimera Solutions, consists of Derek Supino,Jade Adams, and Wayne Harrison. We were tasked with building a reccomendation system on Python for Cinemania's streaming service. We received 4 datasets, icluding a dataset of ratings on a scale of 1-5. 

We use user reviews of movies to build a user-user collaborative modelling system with the Surprise library. By using grid searches and iterating through the potential algorithms, we were able to find the bst models and paramaters for predicting user ratings and providing movie reccomendations. Our final model is a Singular Value Decomposition algorithm that predicts a users rating of a movie within .64 of their actual rating.

We also investigate how we can provide reccomendations with brand new users with no previous reviews, i.e. the 'cold start solution'. For this situation, we use an item-item correlation scores to provide similar movies. Over time, as users rate movies, we can provide more accurate and diverse reccomendations.

Lastly, we investigate the genres with the highest number of reviews and reccommend that Cinemania hones in on providing these to users.

Please go to the main notebook to see our work as a whole. And comment or email us with any feedback :)