# Python_With_Flask_Deployment

This repository contains a sample code to test out deployment of a basic ML model using Python flask framework. Flask is a small and lightweight Python web framework that provides useful tools and features that make creating web applications in Python easier. It gives developers flexibility and is a more accessible framework for new developers since we can build a web application quickly using only a single Python file.

The individual files are described as follows:

model.py - This python script is used to create a basic machine learning (ML) model to predict employee salaries based on data present 'hiring.csv' file which is used to train the model.

app.py - This python script contains Flask APIs which receives employee details through GUI or API calls, computes the predicted value based on our model and returns it.

request.py - This python script uses requests module to call APIs already defined in app.py and displays the returned value.

templates - This folder contains the HTML template to allow user to enter employee detail and displays the predicted employee salary.


### Execution Steps

1) Create the machine learning model by running below command:

python model.py

This would create a serialized version (binary file) of our model into a file named model.pkl.

2) Run app.py using below command to start Flask API
 
python app.py

By default, flask will run on port 5000.

3) Navigate to URL http://localhost:5000
We should be able to view the homepage as below : alt text

Enter valid numerical values in all 3 input boxes and hit Predict.

If everything goes well, we should be able to see the predcited salary vaule on the HTML page! alt text

Direct POST requests can also be sent to the FLask API using Python's inbuilt request module.

Run the below command to send the request with some pre-populated values:

python request.py
