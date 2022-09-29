# “Alexa, Can You Handle Big Data?”


## Background

Many of Amazon's shoppers depend on product reviews to make a purchase. Amazon makes these datasets publicly available. They are quite large and can exceed the capacity of local machines. One dataset alone contains over 1.5 million rows; with over 40 datasets, data analysis can be very demanding on the average local computer. My first goal for this project was be to perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. The second goal was to use PySpark or SQL to perform a statistical analysis of selected data.

This project contained two levels. I have completed the first level.

1. Create DataFrames to match production-ready tables from two big Amazon customer review datasets.

2. Analyze whether reviews from Amazon's Vine program are trustworthy.

- - -


### Level 1

In Level 1 I ...

* Created tables in my RDS database with the provided schema.

* Created two separate Google Colab notebooks and **extracted** two datasets from the list at [review dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), and added each dataset into its own notebook.


* For each notebook I completed the following steps (one dataset per notebook).

  * Counted the number of records (rows) in the dataset.

  * Transformed the dataset to fit the tables in the [schema file](../Resources/schema.sql). 

  * Loaded the DataFrames that correspond to tables into an RDS instance. 







