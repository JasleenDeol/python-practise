# Pandas
## Pandas DataFrame :
- Example :
```
import pandas 

mydataset = {
    "cars": ["BMW", "Volvo", "Ford"],
    "passings": [3,7,2]
}

myvar= pandas.DataFrame(mydataset)
print(myvar)
```
- Output :
```
    cars  passings
0    BMW         3
1  Volvo         7
2   Ford         2
```
## Pandas Series :
- Example :
```
import pandas as pd
a= [1,7,5]
myvar= pd.Series(a)
print(myvar)
```
- Output :
```
0    1
1    7
2    5
dtype: int64
```
## Pandas labels :
- Example :
```
import pandas as pd

a= [1,7,2]

myvar= pd.Series(a,index= ["x","y","z"])

print(myvar["y"])
print(myvar["x"])
```
- Output :
```
7
1
```
