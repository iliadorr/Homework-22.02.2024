# Homework-22.02.2024
Homework for Mr Tauheed

#1 question:
# str, bool, int, float can be used while creating a series object in pandas
# 2 question
import pandas as pd
import numpy as np

mon_number = np.arange(1, 13)

mon_name  = ['January', 'February', 'March', 'April', 'May', "June", 'July', 'August', 'September', 'October', 'November', 'December']

mon_series = pd.Series(data=mon_number, index=mon_name)

print(mon_series)
