# import pandas libary
import pandas as pd
import numpy as np
# Adding Dataset
import pandas as pd
other path = "https://file:///C:/Users/Jinku/Downloads/PY0101EN-1-1-Write_your_first_python_code.ipynb"
# the first 5 rows 
print("the first 5 rows of the dataframe)df.head(5)
# the bottom 10 rows
df.tai(10)
# Creat headers list
headers = ["symboling","normalized-losses","make","fuel-type","aspiration","num-of-dorrs","body-style","driver-wheels","engine-location","wheel-base","length","width","hight","care-weight","engine-type","num-of-cylinders",'engine-size","fuel-system","bore","stroke","comprssion-ratio","horsepower","preak-rpm","city-mpg","highway-mpg","price"]
print("headers\n",headers)
df.column = headers
df.head(10)
# Replace '?'
df1 = df.replace('?',np.Nan)
# drop missing values
df = df1.dropna(subset=["price"],axis=0)
df.head(10)
# cheak the data types
print(df.dtypes)
# Describe all the columns in "df"
dataframe.describe(include = "all")
# Desribe 'length' and 'compression-ratio'
df[['length','compression-ratio']].describe()

#Thank You.
