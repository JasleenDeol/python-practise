# Python Task – Enumerated Iteration Using np.ndenumerate()
## Task
- Write a Python program that:

1. Creates a 2D NumPy array with numbers from 1 to 6.
2. Iterates through the array using np.ndenumerate().
3. Prints each index and value during iteration.
## Solution :
- Code :
```
 import numpy as np
arr= np.array([[1,2,3],[4,5,6]])
for idx,x in np.ndenumerate(arr):
    print("Index" ,idx ,"-> Value", x)
```
- Output :
```
Index (0, 0) -> Value 1
Index (0, 1) -> Value 2
Index (0, 2) -> Value 3
Index (1, 0) -> Value 4
Index (1, 1) -> Value 5
Index (1, 2) -> Value 6
```
