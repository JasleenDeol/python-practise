## Code :
```
name= "Alice"  
def greet_local():                              # function
    name= "Bob"
    print(f"Hello,{name} from local!")
def greet_global():                             # function
    print(f"hello,{name} from global!")
greet_local()                                   # function calling
greet_global()
```
## Example Output :
```
Hello,Bob from local!
hello,Alice from global!
```
