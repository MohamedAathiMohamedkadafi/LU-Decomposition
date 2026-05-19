# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
```
1.Start the program and import the required libraries (NumPy and SciPy).
2.Define the matrix using NumPy.
3.Use lu() to perform LU decomposition and display the lower and upper triangular matrices.
4.Use lu_factor() and lu_solve() to factorize the matrix and solve the system of equations.
5.Display the solution and end the program. 
```

## Program:
(i) To find the L and U matrix
```
```
<img width="745" height="331" alt="592300829-01313e8c-905a-45d2-b99a-ab6ac25cf6a2" src="https://github.com/user-attachments/assets/827e018f-7da6-4fdc-9f1a-b87c12b76b31" />

```
/*
Program to find the L and U matrix.
Developed by: Mohamed Aathil M
RegisterNumber: 212225040246
*/

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
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

<img width="1191" height="451" alt="592301565-3cd47130-64d5-42a5-9abb-3ea0c693aa7c" src="https://github.com/user-attachments/assets/5e733dba-3fd1-44dc-8da4-edb0ab256ec1" />



(2)

<img width="930" height="181" alt="592301721-29fce789-1fad-4c40-a406-23d754dfe925" src="https://github.com/user-attachments/assets/2c300340-8572-433d-b3d9-a354ae95bb46" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

