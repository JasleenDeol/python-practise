# Python Task – NumPy Copy, View & Iteration
## Task
Write a Python program using NumPy that demonstrates:

1. The difference between copy and view.
2. Iterating over a 1D array.
3. Iterating over a 2D array (row-wise and element-wise).
## Solution
## Code :
```
import numpy as np
arr= np.array([1,2,3,4,5])
x= arr.copy()
y= arr.view()
arr[0]= 99

print("After Modifing Original Array:")
print("Original array:",arr)
print("Copy (Independent):",x)
print("View (changes reflected):",y)
print("Iterating over 1d array:")

for x in arr:
    print(x)
```
## Sample Output :
```
After Modifing Original Array:
Original array: [99  2  3  4  5]
Copy (Independent): [1 2 3 4 5]
View (changes reflected): [99  2  3  4  5]
Iterating over 1d array:
99
2
3
4
5
```
## Code :
```
import numpy as np
arr= np.array([[10,20,30],[40,50,60]])
print("2D Array:",arr)
print("Iterating Row-wise:")    
for x in arr:
    print(x)
    
print("Element Wise:")    

for x in arr:
    for y in x:
        print(y)
```
## Sample Output :
```
2D Array: [[10 20 30]
 [40 50 60]]
Iterating Row-wise:
[10 20 30]
[40 50 60]
Element Wise:
10
20
30
40
50
60
```
