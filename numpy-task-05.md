# Python Task – Iteration in 3D NumPy Arrays
## Task
Write a Python program using NumPy that demonstrates iteration in 3D arrays:
1. Create a 3D array.
2. Iterate over the 2D sub-arrays.
3. Iterate over the 1D arrays inside each 2D sub-array.
4. Iterate element-wise through the entire 3D array.
# Solution
## Code : 
```
import numpy as np
arr= np.array([[[1,2,3],[4,5,6]],[[7,8,9],[10,11,12]]])
print("3d array:",arr)

print("Iterating over 2-D arrays:")
for x in arr:
    print(x)
    
print("Iterating over 1D arrays inside each 2d arrays:")
for x in arr:
    for y in x:
        print(y)
        
print("Iterating element wise through entire 3d array:")
for x in np.nditer(arr):
    print(x)
```
## Sample Output :
```
3d array: [[[ 1  2  3]
  [ 4  5  6]]

 [[ 7  8  9]
  [10 11 12]]]
Iterating over 2-D arrays:
[[1 2 3]
 [4 5 6]]
[[ 7  8  9]
 [10 11 12]]
Iterating over 1D arrays inside each 2d arrays:
[1 2 3]
[4 5 6]
[7 8 9]
[10 11 12]
Iterating element wise through entire 3d array:
1
2
3
4
5
6
7
8
9
10
11
12
```
