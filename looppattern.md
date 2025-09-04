## Patterns
```
1) t= 5
   for x in range (1,t+1):
       print("*"*x)
```
- Example Run
```
 *
 **
 ***
 ****
 *****
```
```
2) t=int(input("enter number of rows:"))
   for x in range (1,t+1):
       for y in range (1,x+1):
           print(y,end="")
       print()
```
- Example Run
```
enter number of rows: 8
1
12
123
1234
12345
123456
1234567
12345678
```
```
3) rows=int(input("enter number of rows:"))
   for i in range(rows):
       print(" "*(i),end="")
       print("*" * (2*(rows-i)-1))
```
- Example Run
```
enter number of rows: 5
*********
 *******
  *****
   ***
    *
```  
```
4) rows= int(input("Enter number of rows:"))
   for i in range(rows):
       print(" "*(rows-i-1),end="")
       print("*" * (2 *i+1))
```
- Example Run
```
  Enter number of rows: 5
    *
   ***
  *****
 *******
*********
```
