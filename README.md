**Film Franchise Box Office Predictor**

Over the past decades, we see that film franchises has been around due to critics and audiences response for more sequels. For more sequels, it would mean that the box office needs to show profit for studios to greenlit more sequels based on how the film is received.

We are going to look into Box Office Revenue for film franchises only in U.S. and Canada based on the dataset I created.


The dataset, Film Franchise Box Office Revenue (US and Canada) includes:

* Franchise - Film Title for Franchise
* Total - Total revenue for film franchise
* Releases - The number of releases where the franchise includes re-releases and sequels
* Top Release - The film in the film franchise that made the most profit
* Domestic Lifetime Gross - How much the film has made in the franchise
* Budget - How much did the film cost?
* Studio - The film that was produced and distributed from?
* Rating - The classification rating for the film
* Average Critic Score - The number of critics who like the film
* Average Audience Score - The number of audiences who like the film
* Main Actor - The lead actor who stars in the film

**Process**
* First, we look at our datatypes and check to see if changes need to make on dataset. We also checked to see if any null values are present.
* We encoded our columns that we needed for prediction model such as **Studio**, **Main Actor**, and **Rating**
* We then created a new table to split the data and train the model. Model we used included **Random Forest Regressor**, **Gradient Boosting Regressor**, **Ridge Regression**, **Support Vector Regression**
* To improve on accuracy, we did the same models with Hyperparameter Tuning
* Tested a new film with a model with the best accuracy

**Conclusion**

We found that Random Forest Regressor with Hyperparameter Tuning was our best model with an accuracy score of 77%. In order to improve on our accuracy, we can try to add more features to the dataset such as genres, and directors. We can also try to focus on individual original films instead of films that connect to film franchises.

**Sources**
* Box Office Mojo - https://www.boxofficemojo.com/franchise/?ref_=bo_nb_gs_secondarytab
* iMDB - https://www.imdb.com/
* Metacritic - https://www.metacritic.com/
* Wikipedia - https://www.wikipedia.org/
* RottenTomatoes - https://www.rottentomatoes.com/
