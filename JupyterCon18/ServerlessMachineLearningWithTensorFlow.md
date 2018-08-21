# 2018-08-21

## computing resource qwiklabs with google cloud
* https://googlecloud-run.qwiklab.com/home

* https://googlecloud-run.qwiklab.com/classrooms/2211/labs/17778

* data lab is a hosted jupyter environment hosted on google - https://cloud.google.com/datalab/

]$ datalab create my vm

]$ gcloud config set project qwiklabs-gcp-8965620d23555094

]$ datalab create mydatalabvm

]$ select zone 3

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


