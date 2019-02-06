Data Science Topics


A survey was conducted to gauge an audience interest in different data science topics, namely:

Big Data (Spark / Hadoop)
Data Analysis / Statistics
Data Journalism
Data Visualization
Deep Learning
Machine Learning

The participants had three options for each topic: Very Interested, Somewhat interested, and Not interested. 2,233 respondents completed the survey.
A survey was conducted to gauge an audience interest in different data science topics, namely:
​
Big Data (Spark / Hadoop)
Data Analysis / Statistics
Data Journalism
Data Visualization
Deep Learning
Machine Learning
​
The participants had three options for each topic: Very Interested, Somewhat interested, and Not interested. 2,233 respondents completed the survey.
1) Getting and Cleaning the Data

The survey results have been saved in a csv file and can be accessed through this link: https://cocl.us/datascience_survey_data.

The first column represents the data science topics and the first row represents the choices for each topic.

I use the pandas read_csv method to read the csv file into a pandas dataframe.

In order to read the data into a dataframe like the above, one way to do that is to use the index_col parameter in order to load the first column as the index of the dataframe. Here is the documentation on the pandas read_csv method: https://pandas.pydata.org/pandas-docs/stable/generated/pandas.read_csv.html


import pandas as pd
df=pd.read_csv('https://cocl.us/datascience_survey_data')
df.head()
df.columns = ['Topics','Very Interested','Somewhat Interested','Not Interested']
df.head()
Topics	Very Interested	Somewhat Interested	Not Interested
0	Big Data (Spark / Hadoop)	1332	729	127
1	Data Analysis / Statistics	1688	444	60
2	Data Journalism	429	1081	610
3	Data Visualization	1340	734	102
4	Deep Learning	1263	770	136



