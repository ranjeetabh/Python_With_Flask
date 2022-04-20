# Python_With_Flask_Deployment

This repository contains a sample code to test out deployment of a basic ML model using Python flask framework. Flask is a small and lightweight Python web framework that provides useful tools and features that make creating web applications in Python easier. It gives developers flexibility and is a more accessible framework for new developers since we can build a web application quickly using only a single Python file.

The individual files are described as follows:

model.py - This python script is used to create a basic machine learning (ML) model to predict employee salaries based on data present 'hiring.csv' file which is used to train the model.

app.py - This python script contains Flask APIs which receives employee details through GUI or API calls, computes the predicted value based on our model and returns it.

request.py - This python script uses requests module to call APIs already defined in app.py and displays the returned value.

templates - This folder contains the HTML template to allow user to enter employee detail and displays the predicted employee salary.
