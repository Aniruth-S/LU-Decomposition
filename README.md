# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
## Step 1: Import the numpy module to use the built-in functions for calculation
## Step 2: Prepare the lists from each linear equations and assign in np.array()
## Step 3: Using the lu(), we get three results (first is P, second is L and third is U) of the given matrix.
## Step 4: Define a package as "from scipy.linalg import lu_factor, lu_solve" and create the variable as 'X' include the package in that variable.
## Step 5: rint the results L and U matrices or solution X matrix.

## Program:
**(i) To find the L and U matrix**
```

'''Program to find L and U matrix using LU decomposition.
Developed by: Aniruth S
RegisterNumber: 212225040020
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
**(ii) To find the LU Decomposition of a matrix**
```
'''Program to solve a matrix using LU decomposition.
Developed by: Aniruth S
RegisterNumber: 212225040020
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)

```

## Output:

<img width="1437" height="817" alt="{E65BBC1B-316F-4F0B-A240-CAB4D38CC8FF}" src="https://github.com/user-attachments/assets/ee389b76-1739-4168-8d9e-5860c3d46960" />
<img width="1450" height="597" alt="{E455F20E-02B5-4BD2-93AE-9D75FC785BFC}" src="https://github.com/user-attachments/assets/ff7bc211-a9e7-48c8-b5e6-43f56cd93ae2" />


<img width="1448" height="720" alt="{E50C550E-151A-4167-A708-D67330B94004}" src="https://github.com/user-attachments/assets/24c7d040-ca6b-4571-b8e9-b51384c31271" />
<img width="1459" height="371" alt="{DC4AA423-B330-445C-A9A0-5ADA38DD9240}" src="https://github.com/user-attachments/assets/62255780-ef07-4ca6-9067-bc64d89e2c03" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

