# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
```
PROGRAM:1
1.Import libraries: Import numpy and lu from scipy.linalg.
2.Input matrix: Read a 2D matrix from the user and convert it to a NumPy array.
3.Perform decomposition: Use lu() to decompose the matrix into P, L, and U.
4.Extract results: Get the lower triangular matrix L and upper triangular matrix U.
5.Display output: Print the L and U matrices.

PROGRAM:2
1.Input matrix and vector: Define matrix A and right-hand side vector b.
2.LU decomposition: Decompose A into P, L, and U using scipy.linalg.lu().
3.Apply permutation: Compute Pb = P × b to apply row swaps from the permutation matrix.
4.Solve triangular systems:
  Solve L · y = Pb for intermediate vector y.
  Solve U · x = y to get the final solution x.
5.Output solution: Print the solution vector x.
```

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

