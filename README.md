# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

### Algorithm
## (i) To find the L and U matrix
# Step1:
In first step imports the required libraries: NumPy for numerical operations and 'lu' function from SciPy's linear algebra module for LU decomposition.
# Step2:
In second step the line prompts the user to enter a matrix. The 'eval' function is used to evaluate the input as a Python expression, and 'np.array' converts it into a NumPy array.
# Step3:
In third step the 'lu' function is used to perform LU decomposition on the input matrix 'A'. It returns three matrices: 'P' (permutation matrix), 'L' (lower triangular matrix), and 'U' (upper triangular matrix).
(ii) To find the LU Decomposition of a matrix.
# step4:
In fourth step the line prints the lower triangular matrix 'L' obtained from the LU decomposition.
# Step5:
In fifth step the line prints the upper triangular matrix 'U' obtained from the LU decomposition.
# Step6:
End program.
## (ii) To find the LU Decomposition of a matrix
# Step1:
In first step imports the required libraries: NumPy for numerical operations and lu_factor, lu_solve functions from SciPy's linear algebra module.
# Step2:
In second step the line defines a 3x3 matrix A and a 1D array b.
# Step3:
In third step the  lu_factor function is used to perform LU factorization on the matrix A. It returns the factors lu and piv (pivot indices).
# Step4:
In fourth step the lu_solve function is used to solve the system of linear equations using the LU factorization. It takes the LU factorization lu, pivot indices piv, and the right-hand side vector b as inputs and returns the solution vector x.
# Step5:
In fifth step the line prints the solution vector 'x' obtained by solving the system of linear equations.
# Step6:
End program.
## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Ganesh.D
RegisterNumber: 23013987
*/
# To print L and U matrix=
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Ganesh.D
RegisterNumber: 23013987
*/
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A=np.array([[3,2,7],[2,3,1],[3,4,1]])
b=np.array([4,5,7])
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),b)
print(x)
```

## Output:
# To find the L and U matrix
![Alt text](<lu1 .png>)
# To find the LU Decomposition of a matrix
![Alt text](lu2.png)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.
Hence, the program is successfully executed.

