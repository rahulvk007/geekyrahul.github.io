---
layout: post
title: Python Simple Linear Regression Code
author: Rahul
categories: python
permalink: /:categories/:title
comments: false
---

```python
import pandas as pd

import numpy as np
from sklearn.model_selection import train_test_split 
from sklearn.linear_model import LinearRegression
from sklearn import metrics
import matplotlib.pyplot as plt
from matplotlib import style

style.use('ggplot')

df = pd.read_csv('datafile.csv')
#replace datafile.csv with your csv file

print(df.head(25))

x = df[['High Price','Open Price','Low Price','Total Traded Quantity']].values
y = df['Close Price'].values

x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=0)

regressor = LinearRegression()
regressor.fit(x_train,y_train)

print(regressor.coef_)

y_pred = regressor.predict(x_test)
result = pd.DataFrame({'Actual':y_test.flatten(),'Predicted':y_pred.flatten()})
result.head(25)

print('Mean Absolute Error:', metrics.mean_absolute_error(y_test, y_pred))  
print('Mean Squared Error:', metrics.mean_squared_error(y_test, y_pred))  
print('Root Mean Squared Error:', np.sqrt(metrics.mean_squared_error(y_test, y_pred)))

```
If you have any doubts or run into any problem feel free to ask them at our youtube video comments <a href='https://youtu.be/aqhVg3IZyaQ'>here</a>
