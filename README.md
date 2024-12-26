# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i) To find the L and U matrix

1. Import numpy and scripy.linalg , in linalg you can input lu. and in second program can import lu_factor and lu_solve from python library as same as in second program.
2. Get input from user of nested list to compute numpy array format.
3. Define a package as "from scipy.linalg import lu_factor, lu_solve" and create the variable as 'X' include the
 package in that variable.
4. print the b variable to get output (l_matrix)
5. print the b variable to get output (U_matrix)

(ii) To find the LU Decomposition of a matrix

1. In second program can import lu_factor and lu_solve from python library as same as in second program.   
2. Get input from user of nested list to compute numpy array format and declare it both the variable.
3. Create the variable to use input array to compute of lu_factor of matrix variable.
4. Create the new variable for lu_solve to compute of 'x' variable and 'b' variable.
print the corresponding variable (solution) to get output. 
## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Rasindhan R
RegisterNumber:24005508 
'''
import numpy as np 
from scipy.linalg import lu
matrix=np.array(eval(input()))
piv,l_matrix,u_matrix=lu(matrix)
print(l_matrix)
print(u_matrix)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Rasindhan R
RegisterNumber:24005508
'''
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
b=np.array(eval(input()))
x=lu_factor(matrix)
solution=lu_solve(x,b)
print(solution)
```

## Output:
![Output](<exp-5 (1).png>)
![Output](<exp-5 (2).png>)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

