# ML-predict-salary-anaysis

## ML Model Flask-Deployment
This is a demo project to elaborate how Machine Learn Models are deployed on production using Flask API

## Prerequisites

* Scikit Learn
* Pandas
* Numpy
* Flask

## Project Structure
This project has four major parts :

* model.py - This contains code for our Machine Learning model to predict employee salaries based on data in 'hiring.csv' file.
* app.py - This contains Flask APIs that receives employee details through GUI or API calls, computes the precited value based on our model and returns it.
* request.py - This uses requests module to call APIs already defined in app.py and dispalys the returned value.
* templates - This folder contains the HTML template to allow user to enter employee detail and displays the predicted employee salary.
* static - This folder contains the css folder with (style.css) file which has the styling required for out index.html file.

## Running the project
Ensure that you are in the project home directory. Create the machine learning model by running below command
  
    `python model.py`
  
This would create a serialized version of our model into a file model.pkl

Run app.py using below command to start Flask API 

    `python app.py`
  
By default, flask will run on http://127.0.0.1:5000/ (localhost)

Navigate to URL http://127.0.0.1:5000/ (localhost)

## Deployment in Heroku

I have Deployed the api in Heroku, [Click here](https://ml-salary-prediction.herokuapp.com/)
