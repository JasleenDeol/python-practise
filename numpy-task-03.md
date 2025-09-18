#  Python Task – NumPy Basics
## Task
1. Import the NumPy library.
2. Create a NumPy array of numbers from 1 to 10.
3. Perform the following operations:
4. Find the sum, mean, max, and min of the array.
5. Multiply all elements by 2.
6. Create a reshaped 2D array (2x5) from the original array.
# Solution
## Code : 
```
import numpy as np
arr= np.array([1,2,3,4,5,6,7,8,9,10])
print("Original Array:",arr)

s= np.sum(arr)
p= np.mean(arr)
q= np.max(arr)
r= np.min(arr)
t= 2*arr

print("sum:",s)
print("mean:",p)
print("max:",q)
print("min:",r)
print("array multiplied by 2:",t)

x= arr.reshape(2,5)
print("Reshaped 2x5 array:",x)
```
## Sample Output
```
Original Array: [ 1  2  3  4  5  6  7  8  9 10]
sum: 55
mean: 5.5
max: 10
min: 1
array multiplied by 2: [ 2  4  6  8 10 12 14 16 18 20]
Reshaped 2x5 array: [[ 1  2  3  4  5]
                     [ 6  7  8  9 10]]
```
