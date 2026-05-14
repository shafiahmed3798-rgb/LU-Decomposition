# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the numpy module to use the built-in functions for calculation
2. Prepare the lists from each linear equations and assign in np.array()
3. Using the np.linalg.solve(), we can find the solutions.
4. End the program.

## Program:
(i) To find the L and U matrix
```

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
P,L,U=lu(a)
print(L)
print(U)
'''Program to find L and U matrix using LU decomposition.
Developed by: SHAFI AHMED M S
RegisterNumber: 212225240143
'''
```
(ii) To find the LU Decomposition of a matrix
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,pivot=lu_factor(a)
x=lu_solve((lu,pivot),b)
print(x)
'''Program to solve a matrix using LU decomposition.
Developed by: SHAFI AHMED M S
RegisterNumber: 212225240143
'''
```

## Output:
![lu decomposition]()
(i)

<img width="1190" height="462" alt="image" src="https://github.com/user-attachments/assets/de59baf3-782d-4510-b4d0-8367dae80ae0" />

(ii)

<img width="1170" height="224" alt="image" src="https://github.com/user-attachments/assets/89205379-1571-4fe4-9c4f-bf92e4d69f84" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

