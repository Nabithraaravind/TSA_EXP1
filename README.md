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

<img width="1144" height="1095" alt="Screenshot 2025-08-12 093614" src="https://github.com/user-attachments/assets/73f9b188-172d-4b1f-b298-22450bbfedff" />

<img width="1144" height="1095" alt="Screenshot 2025-08-12 093614" src="https://github.com/user-attachments/assets/a04f5b88-bfdc-4051-b36d-e9e9e44599e6" />
<img width="964" height="1099" alt="Screenshot 2025-08-12 093645" src="https://github.com/user-attachments/assets/d2eb785c-64e5-4dea-88ac-f0c0801f385d" />


# RESULT:
Thus we have created the python code for plotting the time series of given data.
