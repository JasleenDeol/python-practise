# Python Task – NumPy Joining Arrays
## Task
- Write a Python program that demonstrates how to join arrays in NumPy:
## Solution
- Code :
```
import numpy as np
arr1= np.array([1,2,3])
arr2= np.array([4,5,6])
x= np.concatenate([arr1,arr2])
print("Joined 1-D array:",x)
```
- Output :
```
Joined 1-D array: [1 2 3 4 5 6]
```
- Code :
```
import numpy as np
arr1= np.array([[1,2],[3,4]])
arr2= np.array([[5,6],[7,8]])
x= np.concatenate([arr1,arr2],axis=0)
print("Joined 2D array (axis=0):")
print(x)

y= np.concatenate([arr1,arr2],axis=1)
print("Joined 2D array (axis=1):")
print(y)
```
- Output :
```
Joined 2D array (axis=0):
[[1 2]
 [3 4]
 [5 6]
 [7 8]]
Joined 2D array (axis=1):
[[1 2 5 6]
 [3 4 7 8]]
```
