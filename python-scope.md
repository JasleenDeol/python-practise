## Python Scope
 Scope : A variable is only available from insie the region it is created. This is called scope. It can be a local scope or a global scope.
 - local scope : A variable created inside a function belongs to the local scope of that function and can only be used inside that function.
```
1) def myfunction():
       x= 300
       print(x)
   myfunction()
```
 Example run:
```
300
```
```
2) def myfunction():
       x= 300
       def myinnerfunction():
           print(x)
       myinnerfunction()
   myfunction()
```
Exmple run:
```
300
```
- Global Scope : A variable created in the main body of the python code is a global variable and belongs to the global scope.
  Global variables are available from within any scope, global and local.
```
x= 300
def myfunction():
    print(x)
    y= 500
    print(y)
myfunction()
print(x)
```
example run:
```
300
500
300
```
