# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Define the package as scipy.linalg import lu.
2. Get input from user and print L and U matrix by 'print' . 
3. Define a package as "from scipy.linalg import lu_factor, lu_solve" and create the variable as 'X' include the package in that variable 
4. print the variable 'X'

## Program:
```python
import numpy as np 
from scipy.linalg import lu 
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
import numpy as np
import scipy.linalg
A = np.array([[3, 2, 7], [2, 3, 1], [3, 4, 1]], dtype=float)
b = np.array([4, 5, 7], dtype=float)
P, L, U = scipy.linalg.lu(A)
Pb = np.dot(P, b)
y = scipy.linalg.solve(L, Pb)
x = scipy.linalg.solve(U, y)
print(x)
```

## Output:

![image](https://github.com/user-attachments/assets/dd1f3fbd-5184-4eab-81e1-2b1bff9a5e71)

![image](https://github.com/user-attachments/assets/d8778210-ae14-4657-8d99-36b04e1d9505)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

