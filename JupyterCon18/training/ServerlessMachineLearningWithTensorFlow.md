# 2018-08-21

$300 for 12 months on a free trial basis.

## computing resource qwiklabs with google cloud
* https://googlecloud-run.qwiklab.com/home

* https://googlecloud-run.qwiklab.com/classrooms/2211/labs/17778

* data lab is a hosted jupyter environment hosted on google - https://cloud.google.com/datalab/

]$ datalab create my vm

]$ gcloud config set project qwiklabs-gcp-8965620d23555094

]$ datalab create mydatalabvm

]$ select zone 3

To Get Back into the system

]$ gcloud config set project qwiklabs-gcp-8965620d23555094
]$ datalab connect mydatalabvm

### lab 1: data and notebook for lab 1 - estimating NYC cab fares
]$ git clone https://github.com/GoogleCloudPlatform/training-data-analyst

datalab/training-data-analyst/courses/machine_learning/datasets/create_datasets.ipynb

### datalab.bigquery
https://googledatalab.github.io/pydatalab/datalab.bigquery.html

eg: bq.Query(<<sql-string>>).to_dataframe()

### lab 2
]$ datalab connect mydatalabvm

datalab/training-data-analyst/courses/machine_learning/tensorflow/a_tfstart.ipynb

* pick an estimator (model = tf.estimator.LinearRegressor)
* do model.train takes def train_input_fn()
* def pred_input_fn() --> out = trained.predict(pred_input_fn)

### lab 3
https://www.tensorflow.org/guide/feature_columns

datalab/training-data-analyst/courses/machine_learning/tensorflow/b_estimator.ipynb

take away: structure of tf estimator

* input function converts data to tensors

### lab 4
datalab/training-data-analyst/courses/machine_learning/tensorflow/c_batched.ipynb
* big data
* feature engineering
* model architecture
* hyper parameter tuning

tensor flow jargon: step == batch

### lab 5 (TensorBoard)
datalab/training-data-analyst/courses/machine_learning/tensorflow/d_traineval.ipynb

tensorboard - way to visualize/monitor training

NB: in notebook the tensorboard cell comes after the train_and_evaluate, should be before so move cell up
NB: tensorboard only works once per notebook so to do it again you ahve to reset notebook


Cloud ML Engine - managed

1. code that can distribute

2. provide distributed environment
  * if you write code with tf distribution you can specify number of nodes etc.
  
  
### Lab 6 (to a distributed environment and cloud deployment of model with REST)
* need to package code in python module (aka make it not a notebook)
  * task.py - parses command line parameters (eg batch size, learning rate)
  * model.py - contains everything else
  * __init__.py
* datalab/training-data-analyst/courses/machine_learning/cloudmle/cloudmle.ipynb

* bucket: alonzi-qwiklabs-gcp-8965620d23555094
* location: us-east1
* let's you deploy model on the cloud to curl at to make predictions

### Lab 7 (feature engineering and hyperparameter tuning)
* feature engineering
  * tf.feature_column.categorical_column_with_vocabulary_list(...) - for onehot where you know the population
  * there is also a version with hash for when you don't know
  * tf.feature_column.crossed_column([a,b],len(a)xlen(b)
  * basically there are buch of tf.feature_columns, just pick the right one

* model architecture
  * wide and deep models with tensor flow
    * feature crosses in linear model - b/c sparse kills neural netowrk --> memorization in linear
    * one hot layer condense into dense layer (embedding) --> generalization in deep
  * DNNLinearCombinedClassifier
    * linear features = wide columns
    * dense features = deep columns
  
* datalab/training-data-analyst/courses/machine_learning/feateng/feateng.ipynb
  * apache beam - api that treats batch and streaming in unified paradigm
  * data flow is an engine that implements apache beam
* didn't get to hyperparameter tuning but there is a ipynb (not a tensorflow thing)
  * need to expose it as a command line parameter
  * add trial id code for no over writing
  * create a .yaml
  * "much more intelligent than grid search", bayes optimization (there is a paper out there)
