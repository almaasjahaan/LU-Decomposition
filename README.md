# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import required libraries numpy and scipy.linalg.

2. Input the matrix/matrices using eval(input()).

3. Perform LU decomposition using lu() or solve equations using lu_factor() and lu_solve().

4. Print the results L and U matrices or solution X matrix.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: M ALMAAS JAHAAN
RegisterNumber: 212224230016
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: M ALMAAS JAHAAN
RegisterNumber: 212224230016
'''
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:
![lu decomposition]()
![image](https://github.com/user-attachments/assets/88fdff95-0d62-4955-bcf1-330670bd413a)
![image](https://github.com/user-attachments/assets/a50ad566-fe91-4592-8537-c87bfe948132)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

