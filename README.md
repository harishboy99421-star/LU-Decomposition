# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. LU Decomposition of a matrix
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner
3. LU Decomposition of a matrix is written and verified using python programming
   
4.Use lu(),lu_solve(),lu_factor() to get the solutions
5.End the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: 
RegisterNumber: 
*/
```
```


import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Harish N
RegisterNumber: 212225220037
*/
```
```

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu , piv),b)
print(X)
```

## Output:
<img width="1276" height="786" alt="Screenshot 2026-08-24 194953" src="https://github.com/user-attachments/assets/974b249f-f571-45a7-9f4e-7c48f577aa37" />
<img width="1340" height="780" alt="image" src="https://github.com/user-attachments/assets/4aa821c2-a54a-4f32-a8e6-222218ad3b7e" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

