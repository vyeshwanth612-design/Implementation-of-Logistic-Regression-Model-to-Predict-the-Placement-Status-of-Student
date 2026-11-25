# Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student

## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import NumPy and LogisticRegression from sklearn.
2. Create the input data (CGPA and Aptitude Score) and output data (Placement Status).
3. Train the logistic regression model using the fit() function.
4. 1. Predict the student's placement status using the predict() function and display the result.

## Program:
```py

import numpy as np
from sklearn.linear_model import LogisticRegression

X = np.array([[5, 50], [6, 60], [7, 65], [8, 75], [9, 85], [5.5, 55], [7.5, 70], [8.5, 80]])
Y = np.array([0, 0, 0, 1, 1, 0, 1, 1])

model = LogisticRegression()
model.fit(X, Y)

prediction = model.predict([[7.8, 72]])

if prediction[0] == 1:
    print("Student is Placed")
else:
    print("Student is Not Placed")

```

## Output:
<img width="166" height="42" alt="image" src="https://github.com/user-attachments/assets/398bae5f-5e5d-4a97-aee6-82890737eeab" />


## Result:
Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
