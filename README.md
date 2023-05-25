# A Crash Course in PySpark (from Udemy Business)

## Contents :
#### DataIngestionCleaningPySpark.py
* Installation of Spark
* Data Ingestion
* Data Cleaning
#### DataIntoDataFramesPySpark.py
* Bringing Data into Dataframe
* Inspecting a DataFrame
* Handling Null & Duplicate Values
* Selecting & Filtering Data
* Running SQL DataFrames
* Adding Calculated Columns
* GroupBy & Aggregation
* Writing Dataframes to Files

#### Installation
* !apt-get install openjdk-8-jdk-headless -qq > /dev/null
* !wget -q http://archive.apache.org/dist/spark/spark-3.1.1/spark-3.1.1-bin-hadoop3.2.tgz
* !tar xf spark-3.1.1-bin-hadoop3.2.tgz
* !pip install -q findspark
* import os
* os.environ["JAVA_HOME"] = "/usr/lib/jvm/java-8-openjdk-amd64"
* os.environ["SPARK_HOME"] = "/content/spark-3.1.1-bin-hadoop3.2"
* import findspark
* findspark.init()
* from pyspark.sql import SparkSession
* spark = SparkSession.builder.master("local[*]").getOrCreate()
* spark
