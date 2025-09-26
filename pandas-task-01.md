# Pandas Series :
## Code :
```
import pandas as pd
arr= [10,20,30,40,50]
newarr= pd.Series(arr,index= ["a","b","c","d","e"])
print("Series :")
print(newarr)
print()

x= newarr["c"]
print("Value at index 'c' :",x)
print()

import numpy as np
x= np.sum(newarr)
print("Sum :",x)
print()
            # or

x= pd.Series(sum(newarr))
print("Sum:",x)
print()

import numpy as np
x= np.mean(newarr)
print("Mean :",x)
print()

x= newarr*(2)
print("Series*2 :")
print(x)
```
## Output :
```
Series :
a    10
b    20
c    30
d    40
e    50
dtype: int64

Value at index 'c' : 30

Sum : 150

Sum: 0    150
dtype: int64

Mean : 30.0

Series*2 :
a     20
b     40
c     60
d     80
e    100
dtype: int64
```
# Pandas DataFrame :
## Code :
```
import pandas as pd
data = {
    
    "Name":["John","Alice","Bob","Emma","David"],
    "Age":[20,19,21,22,20],
    "Marks":[85, 92,75,90, 60],
    "City":["New York","London","Paris","Tokyo", "Sydney"]
}



y= pd.DataFrame(data)
print(y)  
print()

print("First three rows:")    
print(y.head(3))   

print()
print(y[["Name","Marks"]])

print()
print(y[y["Marks"]>80])
```
## Output :
```
   Name  Age  Marks      City
0   John   20     85  New York
1  Alice   19     92    London
2    Bob   21     75     Paris
3   Emma   22     90     Tokyo
4  David   20     60    Sydney

First three rows:
    Name  Age  Marks      City
0   John   20     85  New York
1  Alice   19     92    London
2    Bob   21     75     Paris

    Name  Marks
0   John     85
1  Alice     92
2    Bob     75
3   Emma     90
4  David     60

    Name  Age  Marks      City
0   John   20     85  New York
1  Alice   19     92    London
3   Emma   22     90     Tokyo
```
# Reading CSV & JSON :
## Code :
```
import pandas as pd
x= pd.read_csv("students.csv")
print(x)
```
## Output :
```
    Name  Age  Marks      City
0   John   20     85  New York
1  Alice   19     92    London
2    Bob   21     75     Paris
3   Emma   22     90     Tokyo
4  David   20     60    Sydney
```
## Code :
```
import pandas as pd
x= pd.read_json("student.json")
print(x)
```
## Output :
```
    Name  Age  Marks      City
0   John   20     85  New York
1  Alice   19     92    London
2    Bob   21     75     Paris
3   Emma   22     90     Tokyo
4  David   20     60    Sydney
```
