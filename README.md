# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 12-08-2025

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:

import pandas as pd
import matplotlib.pyplot as plt

df=pd.read_csv('DailyDelhiClimateTest.csv')
df.shape

df1=df.head(100)
df1
df.info()
df.describe()
x=df1['date']
y=df1['meanpressure']

plt.figure(figsize=(10,6))
plt.bar(x,y)
plt.grid(True)
plt.title('date vs meanpressure')
plt.xlabel('date')
plt.ylabel('meanpressure')
plt.show()


# OUTPUT:

<img width="1144" height="1095" alt="image" src="https://github.com/user-attachments/assets/06153cb8-cf6c-4742-93a1-b3db998ead80" />

<img width="964" height="1099" alt="image" src="https://github.com/user-attachments/assets/9aba435a-812d-489c-b06f-51fc917943db" />

<img width="1296" height="1103" alt="image" src="https://github.com/user-attachments/assets/a822bb4c-4526-4df9-9733-e1e7788e48e6" />




# RESULT:
Thus we have created the python code for plotting the time series of given data.
