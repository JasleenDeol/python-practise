# Code :
```
import numpy as np

arr= np.array([15, 5, 25, 10, 20, 30])
print("1D Array :",arr)
print()

arr1= np.array([[7,8,9],[4,5,6]])
print("2D Array :")
print(arr1)
print()

print("2nd Element of 1d array :",arr[1])
print("Element at row=0, col=2 of 2D array:",arr1[0,2])
print()

print("Sliced 1d array [5,25,10]:",arr[1:4])
print()

print("Data type of arr1:",arr1.dtype)

newarr= arr.astype('f')
print("Converted to float:", newarr)
print()

newarr1= arr.reshape(2,3)
print("Reshaped 2x3 Array:")
print(newarr1)
print()

print("Enumerating reshaped array:")
for idx,x in np.ndenumerate(newarr1):
    print("Index",idx, "-> Value",x)
print()

x= np.array([30,40])
newarr= np.concatenate([arr,x])
print("Concatenated 1D array:",newarr)
print()

print("Stacked Arrays (axis= 0):")
x= np.array([[1,2,3],[4,5,6]])
newarr= np.stack(x,axis= (0))
print(newarr)
print()

print("Stacked array (axis= 1) :")
newarr= np.stack(x,axis=(1))
print(newarr)
print()

print("Splitted 1d array in 3 parts:")
newarr= np.array_split(arr,3)

for x in newarr:
    print(x)
print()

newarr= np.sort(arr)
print("Sorted 1-D array:", newarr)

newarr= np.sort(arr1)
print("Sorted 2D array row wise:")
print(newarr)
```
# Output :
```
1D Array : [15  5 25 10 20 30]

2D Array :
[[7 8 9]
 [4 5 6]]

2nd Element of 1d array : 5
Element at row=0, col=2 of 2D array: 9

Sliced 1d array [5,25,10]: [ 5 25 10]

Data type of arr1: int64
Converted to float: [15.  5. 25. 10. 20. 30.]

Reshaped 2x3 Array:
[[15  5 25]
 [10 20 30]]

Enumerating reshaped array:
Index (0, 0) -> Value 15
Index (0, 1) -> Value 5
Index (0, 2) -> Value 25
Index (1, 0) -> Value 10
Index (1, 1) -> Value 20
Index (1, 2) -> Value 30

Concatenated 1D array: [15  5 25 10 20 30 30 40]

Stacked Arrays (axis= 0):
[[1 2 3]
 [4 5 6]]

Stacked array (axis= 1) :
[[1 4]
 [2 5]
 [3 6]]

Splitted 1d array in 3 parts:
[15  5]
[25 10]
[20 30]

Sorted 1-D array: [ 5 10 15 20 25 30]
Sorted 2D array row wise:
[[7 8 9]
 [4 5 6]]
```
