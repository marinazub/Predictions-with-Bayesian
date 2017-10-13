# Predictions-with-Bayesian
Develop a Bayesian regression model to predict audience_score from the following explanatory variables.
feature_film: "yes" if title_type is Feature Film, "no" otherwise
drama: "yes" if genre is Drama, "no" otherwise
runtime
mpaa_rating_R: "yes" if mpaa_rating is R, "no" otherwise
thtr_rel_year
oscar_season: "yes" if movie is released in November, October, or December (based on thtr_rel_month), "no" otherwise
summer_season: "yes" if movie is released in May, June, July, or August (based on thtr_rel_month), "no" otherwise
imdb_rating
imdb_num_votes
critics_score
best_pic_nom
best_pic_win
best_actor_win
best_actress_win
best_dir_win
top200_box

* * *

## Part 1: Data
<p> This concludes 651 observations from the independent movie internet-resources such as Rotten Tomatoes and IMDB, random sampled. 651 movies, which are less than 10% of all movies of the cinematographic era and less than 10% of movies on both web resources. So, because data is got from 2 popular movie resources, we should keep in mind that the prediction model, based on the data from this resources, is applicable to make a prediction for them only. It could not be spread through entire population, except IMDB and Rotten Tomatoes web-site variability of which should be considered in a separate work. </p><br>
<p>During this work we'll use Oscar Season and Summer Season, Drama and Featured film  variables to predict movie popularity (audience_score) applying Bayesian Regression model </p>



* * *

## Part 2: Data manipulation
Create new variables using the mutate function in the dplyr package following these guidelines:

Create new variable based on `title_type`: New variable should be called `feature_film` with levels yes (movies that are feature films) and no 
Create new variable based on `genre`: New variable should be called `drama` with levels yes (movies that are dramas) and no 
Create new variable based on `mpaa_rating`: New variable should be called `mpaa_rating_R` with levels yes (movies that are R rated) and no 
Create two new variables based on `thtr_rel_month`:
New variable called `oscar_season` with levels yes (if movie is released in November, October, or December) and no 
New variable called `summer_season` with levels yes (if movie is released in May, June, July, or August) and no

* * *

## Part 3: EDA
Perform exploratory data analysis (EDA) of the relationship between audience_score and the new variables constructed in the previous part. Your EDA should contain numerical summaries and visualizations. This might mean you initially create a lot more visualizations and summary statistics than what you finally choose to include in your paper. Each R output and plot should be accompanied by a brief interpretation

* * *

## Part 4: Modeling
 Develop a Bayesian regression model to predict `audience_score` from the following explanatory variables. Note that some of these variables are in the original dataset provided, and others are new variables you constructed earlier:`feature_film`,` drama`, `runtime`, `mpaa_rating_R`, `thtr_rel_year`, `oscar_season`, `summer_season`, `imdb_rating`, `imdb_num_votes`, `critics_score`, `best_pic_nom`, `best_pic_win`, `best_actor_win`, `best_actress_win`, `best_dir_win`, `top200_box`. Complete Bayesian model selection and report the final model. Also perform model diagnostics and interpret coefficients of your final model in context of the data.

* * *

## Part 5: Prediction
I Picked a Scuicide Sqade  movie  featured in 2016 with the audience score, according to Rotten Tomatoes, 62 https://www.rottentomatoes.com/m/suicide_squad_2016 and did a prediction for this movie using my developed model and the `predict` function in R.

* * *

## Part 6: Summary



