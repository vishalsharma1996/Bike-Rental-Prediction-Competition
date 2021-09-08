# Bike-Rental-Prediction-Competition
This competition is all about predicting the total number of registered and casual rental users for any month(from 20th of that month to the last) for a two year timeframe.
The above repo contains the analysis separately for both registered and casual rental users.It also contains the code for the final submission file.
Here we are able to get the score in top 1% of the private leaderboard.

EDA_BIKE_RENTAL_FE_MODELLING_REGISTERED_USERS & EDA_BIKE_RENTAL_FE_MODELLING_REGISTERED_USERS-->Both the file contains the code for EDA Feature Engineering Feature Selection and hyperparameter tuning.Now one needs to save both the train and test csv files so that it can be used for blending.The final prediction for the casual users is done within the EDA file only which should be saved as a csv file which will be used in the final prediction.

Ensemble(Blending)-->This contains a detailed aprroach where 6 different tree based models are used as base models and a linear regression model is fitted on it.The final test prediction is made by this metal model and be saved as a csv file.

Final_pred-->This file contains the code for our final submission file where we will concatenate the readings from the blended model used for registered users and xgboost model used for the casual users.
