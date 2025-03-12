# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 11.03.25
# Reg no: 212224220012
# Name: Ashwath p

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
```
import pandas as pd
import matplotlib.pyplot as plt
file_path = '/content/fitness_tracker.csv'
data = pd.read_csv(file_path)
data['User_ID'] = pd.to_datetime(data['User_ID'])
data.set_index('User_ID', inplace=True )
plt.figure(figsize=(10, 6))
plt.plot(data.index, data['Steps'], label='Steps', color='blue')
plt.title('fitness tracker')
plt.xlabel('User_ID')
plt.ylabel('Calories_Burned')
plt.grid(True)
plt.legend()
plt.show()
```












# OUTPUT:

![image](https://github.com/user-attachments/assets/ae6aaf5f-b6db-48fc-a25d-3346addf0ec0)







# RESULT:
Thus we have created the python code for plotting the time series of given data.
