# EECS-731---Fall-2020---Assignment-6-Anomaly-Detection

The dataset contains real time traffic data from the Twin Cities Metro area in Minnesota, collected by the Minnesota Department of Transportation. Included metrics include occupancy, speed, and travel time from specific sensors. This dataset has speeds for vehicles captured by different sensors. Here, we have considered the car speeding data only,

The overall goal is to build one or more Build one or more anomaly detection models to determine the anomalies using the other columns as features

The dataset can be found at: https://www.kaggle.com/boltzmannbrain/nab

Reference: References used: 1) http://scikit-learn.org/stable/modules/generated/sklearn.neighbors.LocalOutlierFactor.html
2) https://towardsdatascience.com/outlier-detection-with-isolation-forest-3d190448d45e
3) youtube.com/watch?v=gCWBFyFTxVU
Structure/steps:

A deatiled explanantion at each step is mentioned as we walk down the code and results in the jupyter notebook (uploaded on GitHub).

Steps (Data processing and evalaution) :

Imported required modules

Read the data csv file Initial data analysis and cleaning (checking for null values) Filter the column data based on the requirements that will help to provide visual representations

We will be applying two types of anomaly detection on the data
Isolation Forest
One Class SVM
Local outlier factor

Higher accuracvy score corresponds to a better model. After trying three diffeent classifier models,we observe,

1) Isolation forests detects 1094 errors with an accuracy of 82.13%
2) Local Outlier Factor detects 1535 errors with an accuracy of 74.92%
3) Support Vector Machine detects 2434 errors with an accuracy of 60.24%
4) When comparing error, precision, accuracy score & recall for 3 models , the Isolation Forest performed much better than the LOF and SVM models
