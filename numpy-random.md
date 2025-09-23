## Random Number: 
Random number does not mean a different number. It means something that cannnot be predicted logically
- Code & Output : 
```
# Generating Integer random number
from numpy import random
x= random.randint(100)
print(x)

45
```
```
# Generate float random number
from numpy import random
x= random.rand()
print(x)

0.028948797537725057
```
```
# To generate 1D array (integer)
from numpy import random
x= random.randint(100,size=(5))
print(x)

[79 59 95 89  2]
```
```
# To generate 1d array (float)
from numpy import random
x= random.rand(5)
print(x)

[0.79160219 0.33899706 0.15203026 0.47747458 0.21206094]
```
```
# Generate 2D random (Integer) array
from numpy import random
x= random.randint(100,size=(3,5))
print(x)

[[49 27 86 38 21]
 [65 54  1 83 75]
 [22 23 26 68 10]]
```
```
# Generate random number from array
from numpy import random
x= random.choice([3,5,7,9])
print(x)

7
```
```
# Generate 1D array from array
from numpy import random
x= random.choice([3,5,7,9],size=(5))
print(x)

[7 9 9 9 5]
```
```
# Generate 2D array from array
from numpy import random
x= random.choice([3,5,7,9],size=(3,5))
print(x)

[[9 9 9 9 7]
 [5 7 3 7 9]
 [5 9 5 3 3]]
```
