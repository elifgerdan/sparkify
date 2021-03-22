# Churn Prediction with PySpark


### 1. Project Overview
Our goal is to build and train a binary classifier that is able to accurately identify users (in both free and paid tier) who cancelled the Sparkify music streaming service, based on the patterns obtained from their past activity and interaction with the service. A successfully trained model could be used to identify users who are likely to churn in advance.


### 2. File Descriptions
- `sparkify.ipynb` : Jupyter notebook with all the analyses, modelling steps, code, results, visualizations, plus all supporting discussions and comprehensive documentation

The full Sparkify dataset (12GB) used in this project is hosted on Udacity's publicly available Amazon S3 bucket: `s3n://udacity-dsnd/sparkify/sparkify_event_data.json`

The smaller version used for data exploration (128MB) is available under: `s3n://udacity-dsnd/sparkify/mini_sparkify_event_data.json`


### 3. Results
Accuracy and f1 score are very good. However, it should not be forgotten that the dataset may not be representing all customer base, I used mini — sized dataset. In real world and big data set, I think that 80% accuracy ratio is very good.

I have also calculated feature importance in predicting customer churn. I observe that register_duration (days — customer lifetime), number of thumbs down and average listened songs per session are top 3 important features while predicting churn.

you may see my blogpost here: [Medium](https://elifgerdan.medium.com/sparkify-whyd-you-leave-2455794cd0bb`)

### 4. Libraries
- PySpark version 2.4.3 was used in this project, primarily `pyspark.sql` module for working with structured data and `pyspark.ml` that provides a set of high-level APIs to create practical machine learning pipelines
- no additional libraries have been used beyond the Anaconda distribution of Python, and there should be no issues running the code using Python versions 3.x

### 5. Acknowledgments
I have to give credit to Udacity for designing projects that are as close as possible to real world scenarios.
