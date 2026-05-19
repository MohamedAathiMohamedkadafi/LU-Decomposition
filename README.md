# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Start the program and import the required libraries (NumPy and SciPy).
2.Define the matrix using NumPy.
3.Use lu() to perform LU decomposition and display the lower and upper triangular matrices.
4.Use lu_factor() and lu_solve() to factorize the matrix and solve the system of equations.
5.Display the solution and end the program. 


## Program:
(i) To find the L and U matrix
```
```
<img width="633" height="221" alt="592301146-3c22d992-6a0f-4ea9-8448-a91e25582696" src="https://github.com/user-attachments/assets/073a3f01-b0d2-4034-8315-b45d2544d573" />
```
/*
Program to find the L and U matrix.
Developed by: Mohamed Aathil M
RegisterNumber: 212225040246
*/

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,p=lu_factor(A)
x=lu_solve((lu,p),B)
print(x)

```
(ii) To find the LU Decomposition of a matrix
```


/*
Program to find the LU Decomposition of a matrix.
Developed by:  Mohamed Aathil M
RegisterNumber: 212225040246

*/

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,p=lu_factor(A)
x=lu_solve((lu,p),B)
print(x)
```

## Output:
![lu decomposition]()
(1)




(2)




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

