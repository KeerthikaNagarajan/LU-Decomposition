# LU Decomposition without zero on the diagonal

# 5A

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1:
Import numpy library using import statement.

### Step 2:
From scipy package import lu().

### Step 3:
Get input from user and pass it as an array.

### Step 4:
Get P, L, U matrix using lu()

### Step 5:
Print L and U matrix

## Program:
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Keerthika N
RegisterNumber: 21000385
'''

# To print L and U matrix
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P, L, U = lu(A)
print(L)
print(U)

```

## Output:
![lu decomposition](./5a.png)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.


# 5B

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1:
Import numpy library using import statement.

### Step 2:
From scipy package import lu_factor() and lu_solve().

### Step 3:
Get two inputs from user and pass it as matrix array.

### Step 4:
Find lu and pivot value of first matrix using lu_factor().

### Step 5:
Find solution of the matrix by using lu_solve() by passing lu, pivot values as first argument and second matrix as second argument.

### Step 6:
Print the solution.

## Program:
```
'''Program to solve a matrix using LU decomposition.
Developed by: Keerthika N
RegisterNumber: 21000385
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
B = np.array(eval(input()))
lu, pivot = lu_factor(A)
x = lu_solve((lu,pivot),B)
print(x)

```

## Output:
![lu decomposition](./5b.png)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

