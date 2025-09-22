## Code :
```
import numpy as np
arr = np.array([1,2,3,4,5,6,7,8,9,10,11,12])
x= arr.reshape(3,4)
print("matrix:")
print(x)

arr1=np.array([[ 1,2,3,4],[5,6,7,8],[9,10,11,12]])
x= arr1[1]
print("2nd row:",x)
y= arr1[0:3,3]
print("Last column:",y)
z= arr1[1:3,0:2]
print("sub matrix:")
print(z)

a= arr1*2
print("Matrix multiplied by 2:")
print(a)

arr2 = np.array([[1,2,3,4],[5,6,7,8],[9,10,11,12]])
b= arr1+arr2
print("matrix + other matrix:")
print(b)

c= arr1*arr2
print("Elment-wise multiplication:")
print(c)

d= np.sum(arr1)
print(" Sum of all elements:",d)

e= np.mean(arr1)
print("Mean of all elements:",e)

f= np.max(arr1)
print("max value:",f)

g= np.sum(arr1,axis=0)
print("Sum along axis=0 :",g)

h= np.sum(arr1,axis=1)
print("Sum along axis=1 :",h)
```
## Output:
```
matrix:
[[ 1  2  3  4]
 [ 5  6  7  8]
 [ 9 10 11 12]]
2nd row: [5 6 7 8]
Last column: [ 4  8 12]
sub matrix:
[[ 5  6]
 [ 9 10]]
Matrix multiplied by 2:
[[ 2  4  6  8]
 [10 12 14 16]
 [18 20 22 24]]
matrix + other matrix:
[[ 2  4  6  8]
 [10 12 14 16]
 [18 20 22 24]]
Elment-wise multiplication:
[[  1   4   9  16]
 [ 25  36  49  64]
 [ 81 100 121 144]]
 Sum of all elements: 78
Mean of all elements: 6.5
max value: 12
Sum along axis=0 : [15 18 21 24]
Sum along axis=1 : [10 26 42]
```
