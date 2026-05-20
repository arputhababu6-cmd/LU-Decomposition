# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
Step 1:
Import the numpy module to use the built-in functions for calculation

Step 2:
Prepare the lists from each linear equations and assign in np.array()

Step 3:
Using the np.linalg.solve(), we can find the solutions.

Step 4:
End the program
## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: B ARPUTHA
RegisterNumber: 212225040028
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
p,l,u=lu(matrix)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: B ARPUTHA
RegisterNumber: 212225040028
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu=lu_factor(matrix)
result=lu_solve((piv,lu),constant)
print(result)
```

## Output:
<img width="1188" height="407" alt="image" src="https://github.com/user-attachments/assets/db1ed8f2-db2b-4e5a-a2ca-215f96a7c7bb" />
<img width="855" height="128" alt="image" src="https://github.com/user-attachments/assets/4497a69d-d336-421a-9ef3-92e908974307" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

