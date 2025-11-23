# RAINFALL-DATA-ANALYSER 
A Python project to analyse data and visualise trends.

import pandas as pd 
import matplotlib.pyplot as plt

def analyse_rainfall(file_path)
df= pd.read_csv(file_path)
print("Summary Statistics:\n", df.describe())

plt.figure(figsize=(10,5))
plt.plot(df['Date'], df['Rainfall'], marker='0')
plt.title("Rainfall Trend")
plt.xlabel("Date")
plt.ylabel("Rainfall (mm)")
plt.grid(True)
plt.show()
