## NumPy array basics, including data types, indexing, and slicing.
- Code :
```
import numpy as np
arr= np.array([10,20,30,40,50],dtype='f8')
print("Original Array:",arr)
print("Data Type:",(arr.dtype))


a= arr[0]
b= arr[-1]
print("First Element :",a)
print("Last Element :",b)


d= arr[:3]
e= arr[3:]
f= arr[1:4]
print("First Three Elements:",d)
print("Last Two Elements:", e)
print("Elements from 1st to 3rd :",f)
```
- Output :
```
Original Array: [10. 20. 30. 40. 50.]
Data Type: float64
First Element : 10.0
Last Element : 50.0
First Three Elements: [10. 20. 30.]
Last Two Elements: [40. 50.]
Elements from 1st to 3rd : [20. 30. 40.]
```
