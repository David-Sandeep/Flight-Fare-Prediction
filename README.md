# Flight-Fare-Prediction

## Overview
Flight ticket prices can be something hard to guess, today we might see a price, check out the price of the same flight tomorrow, it will be a different story. We might have often heard travelers saying that flight ticket prices are so unpredictable. As data scientists, we are gonna prove that given the right data anything can be predicted. Here you will be provided with prices of flight tickets for various airlines between the months of March and June of 2019 and between various cities.
This is a Flask web app which predicts fare of Flight ticket.

# Deployed at: https://flightfareprediction0.herokuapp.com/

##  Tech Stack
• Front-End: HTML, CSS.

• Back-End: Flask.

• IDE: Jupyter notebook, Spyder.

## How to run this app
• First create a virtual environment by using this command

• conda create -n myenv python=3.6

• Activate the environment using the below command:

• conda activate myenv

• Then install all the packages by using the following command

• pip install -r requirements.txt

• Now for the final step. Run the app

• python app.py

## Dataset 
Taken from kaggle.

## Steps followed:
• loaded dataset from kaggle.

• Missing Values handled.

• Features extracted like Journey Day,Jounrney month from Date of Journey, from Depature Time extracted features like Departure Hour and Departure minute same from Arrival Time.

• Preprocessed Duration column and extracted Duration hour and minutes.

• We have Categorical Data like Airline,Source,Destination,as  these variables are nominal we performed one-hot-encoding.

• We have Categorical Data like Total_Stops, as it is ordinal we performed label encoding.

• Feature Selection by ExtraTreeRegressor.

• Performed Train Test split.

• Applied Random Forest Regressor.

• used RandomizedSearchCV to perform hyperparameter tuning on Random forest regressor.

• saved the model and deployed in flask.



  • This repository consists of files required to deploy a Machine Learning Web App created with Flask on Heroku platform.
