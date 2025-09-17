# Python Task – NumPy 2D Arrays, Indexing & Slicing
## Task
- Write a Python program using NumPy that demonstrates:

 1. Creating a 2D array with a specific data type.
 2. Accessing elements using row & column indexing.
 3. Extracting sub-arrays using slicing.
## Code :
```
import numpy as np
arr= np.array([[10,20,30],[40,50,60],[70,80,90]],dtype= 'f8')
print("Original Array:",arr)
print("Data Type:",(arr.dtype))


a= arr[0,1]
print("Element at row 0 column 1:",a)

b= arr[2,2]
print("Element at last row last coloumn:",b)

c= arr[0]
print("First Row:",c)

d= arr[0:2,0:2]
print("First two rows and coloumns:",d)

e= arr[0:3,2]
print("Last Column:",e)
```
## Output :
```
Original Array: [[10. 20. 30.]
                 [40. 50. 60.]
                 [70. 80. 90.]]
Data Type: float64
Element at row 0 column 1: 20.0
Element at last row last coloumn: 90.0
First Row: [10. 20. 30.]
First two rows and coloumns: [[10. 20.]
 [40. 50.]]
Last Column: [30. 60. 90.]
```
