# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import required libraries numpy and scipy.linalg.
2. Input the matrix/matrices using eval(input()).
3. Perform LU decomposition using lu().
4. Print the results L and U matrices or solution X matrix

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Mohamed Zabir Khan A
RegisterNumber: 212224230162
'''
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by:Mohamed Zabir Khan A
RegisterNumber: 212224230162
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)
```

## Output:

<img width="1212" height="772" alt="image" src="https://github.com/user-attachments/assets/6778ec12-a0cb-4fbf-a602-a30d06c74dfb" />

<img width="1212" height="772" alt="image" src="https://github.com/user-attachments/assets/d53201ef-3c3f-494e-87fa-a5710b180682" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.
