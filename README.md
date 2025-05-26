# BIG-DATA-ANALYSIS

COMPANY:CODTECH IT SOLUTIONS

NAME:JINKA DEEKSHITHA

INTERN ID:CTO4DF390

DOMAIN:DATA ANALYTICS

DURATION:4 WEEKS

MENTOR:NEELA SANTOSH


Objective:This project focuses on performing big data analysis using PySpark on a large dataset. The dataset used for analysis is related to students' social media addiction. The primary goal is to demonstrate the scalability and performance of PySpark for processing and analyzing large-scale data.
Tool:PySparK 
Technology:Google Colab
used Dataset: Students' Social Media Addiction
About PySpark:
PySpark is the Python interface for Apache Spark, an open-source, distributed computing engine.It enables users to write Spark applications using Python.PySpark is commonly used for big data processing and data analytics.
Installation (Google Colab)
Install PySpark:
!pip install pyspark
Create a Spark Session:
from pyspark.sql import SparkSession
spark = SparkSession.builder.appName("pyspark1").getOrCreate()
Display Spark Session Variable:
spark
now we have to load the dataset to google colab by using below syntax:
df=spark.read.csv('').here we have to copy and paste the dataset path in the parenthesis.
After setting path we can perform different types of operations based on our dataset,and I am using some operations to analyze the dataset like display top 10 rows of the dataset
display datatype of each column
display column names
count number of rows and columns of the dataset
get overall stastics about dataset by using this we can see count,median,mean of our dataset
Display number of students having age greater than 20 etc.,
to find out average for the coloumn avg_daily_usage_hours in the dataset.At firstly we have import sql functions by using the syntax
from pyspark.sql.function import avg after installing sql functions then we have to average the column by using the syntax
df.select(avg("avg_daily_usage_hours")).show()
order or sort data of our dataset by using syntax
df.orderby("conflicts_over_social_media",ascending=true).show() after using this syntax the data get sorted in ascending order.
          


**Output**


![Image](https://github.com/user-attachments/assets/4caf2269-41d9-47ab-ac83-1165f4dcd5cd)
![Image](https://github.com/user-attachments/assets/b8841aa1-26e3-424e-9650-411f5323aa71)
![Image](https://github.com/user-attachments/assets/76528e4e-5be7-4842-831b-facf64230dea)
![Image](https://github.com/user-attachments/assets/81917704-43cd-4df1-baa0-dbb8813b0b5c)
