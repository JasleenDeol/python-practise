# Python Task – NumPy Joining Arrays (concatenate & stack)
## Task
- Write a Python program that demonstrates joining arrays using np.concatenate() and np.stack():
## Solution :
- Code :
```
import numpy as np
arr1= np.array([1,2,3])
arr2= np.array([4,5,6])

x= np.concatenate([arr1,arr2])
print("Concatenated 1D array:",x)

y= np.stack([arr1,arr2],axis=0)
print("Stacked 1D arrays (axis=0):")
print(y)

z= np.stack([arr1,arr2],axis=1)
print("Stacked 1D arrays (axis=1):")
print(z)
```
- Output :
```
Concatenated 1D array: [1 2 3 4 5 6]
Stacked 1D arrays (axis=0):
[[1 2 3]
 [4 5 6]]
Stacked 1D arrays (axis=1):
[[1 4]
 [2 5]
 [3 6]]
```
- Code :
```
import numpy as np
arr1= np.array([[1,2],[3,4]])
arr2= np.array([[5,6],[7,8]])

x= np.concatenate([arr1,arr2],axis=0)
print("Concatenated 2D array (axis=0):")
print(x)

y= np.concatenate([arr1,arr2],axis=1)
print("Concatenated 2D array (axis=1):")
print(y)

z= np.stack([arr1,arr2],axis=0)
print("Stacked 2D array (axis=0):")
print(z)

p= np.stack([arr1,arr2],axis=1)
print("Stacked 2D array (axis=1):")
print(p)
```
- Output :
```
Concatenated 2D array (axis=0):
[[1 2]
 [3 4]
 [5 6]
 [7 8]]
Concatenated 2D array (axis=1):
[[1 2 5 6]
 [3 4 7 8]]
Stacked 2D array (axis=0):
[[[1 2]
  [3 4]]

 [[5 6]
  [7 8]]]
Stacked 2D array (axis=1):
[[[1 2]
  [5 6]]

 [[3 4]
  [7 8]]]
```
