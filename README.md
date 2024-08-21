### Name: Ragul VK
### Register Number: 212221240043
# Ex.No: 01 PLOT A TIME SERIES DATA

# AIM:
To Develop a python program to Plot a time series data temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:


# Temperature:
```python
import matplotlib.pyplot as plt
import pandas as pd
df=pd.read_csv("DailyDelhiClimateTrain.csv",parse_dates=["date"],index_col="date")
df.head()
mean=df["meantemp"].resample('M').mean().plot(kind='line')
plt.xlabel("Month")
plt.ylabel("Temperature")
plt.show()
```


# OUTPUT:
# Temperature:

![4 (1)](https://github.com/JEEVAABI/TSA_EXP1/assets/93427098/dbef86e7-56d2-4d1d-be20-36cd57353f62)



# RESULT:
Thus we have created the Python code for plotting the time series of given data.
