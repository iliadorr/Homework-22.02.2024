# Homework-22.02.2024
Homework for Mr Tauheed

#1 question from Eldiaar
# str, bool, int, float can be used while creating a series object in pandas

# 2 question from Eldiaar
month_data = {
    'January': 1,
    'February': 2,
    'March': 3,
    'April': 4,
    'May': 5,
    'June': 6,
    'July': 7,
    'August': 8,
    'September': 9,
    'October': 10,
    'November': 11,
    'December': 12
}
# 2 step
s = pd.Series(month_data)
# 3 step
print(s)

# 3 question from Eldiiar
import pandas as pd

batch_group = {
    'MatMIE':27,
    'MatDAIS': 30,
    'COMIE':28,
    'COMEC': 34
}

stud_series = pd.Series(batch_group)

print(stud_series)

# 4 question FROM Edliarr

exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
             'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
             'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
             'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j'] 

df = pd.DataFrame(exam_data, index=labels)

print(df)

# 5 question from EldiiR

import numpy as np
import pandas as pd

exam_data = {
    'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
    'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
    'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
    'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']
}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']

df = pd.DataFrame(exam_data, index=labels)

result = df[df['attempts'] > 2]

print("Number of attempts in the examination is greater than 2:")
print(result)
