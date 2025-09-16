# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: pelleti sindhu sri
RegisterNumber: 212224240113

import numpy as np
import matplotlib.pyplot as plt
X = np.array([1, 2, 3, 4, 5])   
Y = np.array([2, 4, 5, 4, 5])   
mean_x = np.mean(X)
mean_y = np.mean(Y)
numerator = np.sum((X - mean_x) * (Y - mean_y))
denominator = np.sum((X - mean_x) ** 2)
m = numerator / denominator
b = mean_y - m * mean_x
print(f"Equation of the line: Y = {m:.2f}X + {b:.2f}")
Y_pred = m * X + b
plt.scatter(X, Y, color="blue", label="Data points")
plt.plot(X, Y_pred, color="red", label="Best fit line")
plt.xlabel("X - Independent Variable")
plt.ylabel("Y - Dependent Variable")
plt.legend()
plt.title("Univariate Linear Regression - Least Squares")
plt.show()

*/
```

## Output:

<img width="727" height="597" alt="Screenshot 2025-09-16 154411" src="https://github.com/user-attachments/assets/f83384e6-0dbf-4d87-a0f0-3492feef9f14" />



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
