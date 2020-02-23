# Sparkify-Project


### Table of Contents

1. [Installation](#installation)
2. [Motivation](#motivation)
3. [Files](#files)
4. [Results](#results)
5. [Licensing](#licensing)

## Installation <a name="installation"></a>
There are two ways to run the attached Project scripts.
<br>
1. Locally 
- You should have Spark installed on your machine
- Python and PySpark API must be installed as well
- Set up all Environment Variables correctly

2. In the Cloud (easier way)
- You should have an Amazon AWS account <br>
(All other requirements are handled by AWS)


## Motivation<a name="motivation"></a>
Sparkify is an imaginary music streaming company with thousands of users which generate vast amounts of data<br>
The data is difficult to analyze on a single machine, due to its volume size<br>
Therefore a Big Data tool such as Spark is needed to analyze this data<br>
The end goal is to predict customer Churn.<br>

The Project code is inside the .ipynb Notebook<br>
The Notebook consists of following parts:

- Importing PySpark modules; Installation of some Python modules
- PySpark session creation
- Data Import
- Data Cleaning
- Data Aggregation and Preparation
- Classification Algorithms are used to predict customer Churn
- Results are evaluated based on common metrics


## Files <a name="files"></a>

Following files are attached to this repository:

- Sparkify_Big.ipynb - Jupyter Notebook with the complete analysis of the full dataset (12GB) <br>
Should be run on Amazon AWS
- Sparkify_Big.html -  the HTML page of the Sparkify_Big.ipynb file

- Sparkify_Small.ipynb - Jupyter Notebook with the analysis of the sample dataset (128MB)
- Sparkify_Small.ipyng - the HTML page of the Sparkify_Small.ipynb file

- mini_sparkify_event_data.zip - sample data set

The Full Data set is stored on the S3 server:
- "s3n://udacity-dsnd/sparkify/sparkify_event_data.json"

Sample Data Set is also available on the S3 server:
- "s3n://udacity-dsnd/sparkify/mini_sparkify_event_data.json"


## Results<a name="results"></a>
sparkify_event_data is a 12GB data set with 25 million rows. It contains user data of about 25K users.<br>

The data contains information about: 
- pages that the user visited
- all timestamps
- time spent on each page
- user gender
- user location
- etc. <br>

The data also contains information whether the user has cancelled the music service or not (Churn)<br>

Data was used to engineer 14 features which served as an input for classification models to predict Churn <br>

Three models were used on the full dataset (12GB), the best performing model was Gradient Boosted Tree Classifier yielding an F1 metric of 0.81 <br>

<b> A detailed step-by-step analysis with results is available here: </b> <br>
https://medium.com/@mihajlovic.aleksa/machine-learning-with-pyspark-and-amazon-emr-3149dbc847ae 

## Licensing<a name="licensing"></a>
The dataset was provided by Udacity https://www.udacity.com/ <br>
For any questions or concerns regarding the dataset, please contact Udacity
