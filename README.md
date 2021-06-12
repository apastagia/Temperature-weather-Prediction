## Randomforest

### Requirement file
pip freeze requirements.txt

pip install -r requirements.txt

Jupyter Notebook1 - Random Forest Approach 
Jupyter Notebook2 - Hypyer Parameter Tuning(Working on Improving Accuracy- by adding more data)
Jupyter Notebook3 - Different approaches used to increase accuracy

Dataset:
temps.csv - for jupyter notebook1
temps_extended.txt - for jupyter notebook2

## Problem Statement
The problem we will tackle is predicting the max temperature using one year of past weather data.

find data for your own city using the https://www.ncdc.noaa.gov/cdo-web/

data file : https://drive.google.com/file/d/1pko9oRmCllAxipZoa3aoztGZfPAD2iwj/view

## Answer

**This is a supervised, regression machine learning problem. It’s supervised because we have both the features (data for the city) and the targets (temperature) that we want to predict. During training, we give the random forest both the features and targets and it must learn how to map the data to a prediction. Moreover, this is a regression task because the target value is continuous (as opposed to discrete classes in classification).**

## Roadmap

1. State the question and determine required data

2. Acquire the data in an accessible format

3. Identify and correct missing data points/anomalies as required

4. Prepare the data for the machine learning model

5. Establish a baseline model that you aim to exceed

6. Train the model on the training data

7. Make predictions on the test data

8. Compare predictions to the known test set targets and calculate performance metrics

9. If performance is not satisfactory, adjust the model, acquire more data, or try a different modeling technique

10. Interpret model and report results visually and numerically

## For creating graph
use pydot/pydotplus and graphviz
Download : https://graphviz.gitlab.io/download/

If this kind of error is generated,
FileNotFoundError: [WinError 2] "dot" not found in path. and '`pydot` failed to call GraphViz.'
https://www.programmersought.com/article/2969856002/

And finally in my notebook I added the two lines below.

import os
os.environ["PATH"] += os.pathsep + 'C:/Program Files/Graphviz2.38/bin/'
