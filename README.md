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
Developed by: syed shahid S
RegisterNumber:  25004343
import numpy as np
import matplotlib.pyplot as plt
x = np.array(eval(input()))
y = np.array(eval(input()))
2,9,5,5,3,7,1,8,6,2
69,98,82,77,71,84,55,94,84,64
x_mean = np.mean(x)
y_mean = np.mean(y)
num = 0
denom = 0
for i in range(len(x)):
num += (x[i] - x_mean) * (y[i] - y_mean)
denom += (x[i] - x_mean) ** 2
m = num / denom
b = y_mean - m * x_mean
Start coding or generate with AI.
print(m, b)
4.742603550295859 55.035502958579876
y_predicted = m * x + b
print(y_predicted)
[64.52071006 97.71893491 78.74852071 78.74852071 69.26331361 88.23372781
 59.77810651 92.97633136 83.49112426 64.52071006]
plt.scatter(x, y)
plt.plot(x, y_predicted, color='red')
plt.show()

*/
```

## Output:
![best fit line](sam.png)
![alt text](<Screenshot 2026-01-31 081943.png>)

## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
