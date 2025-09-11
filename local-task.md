## Code :
```
counter= 0
def increment_global():
    global counter                                     # global keyword
    counter += 1
    print("Global counter:",counter)
def increment_local():
    counter= 0
    counter += 1
    print("Local counter:",counter)
def outer_function():
    counter= 0
    def inner_function():
        nonlocal counter                               # nonlocal keyword
        counter += 1
        print("Nonlocal counter:",counter)
    inner_function()
    print("Outer counter after inner:",counter)
increment_global()
increment_local()
outer_function()
print("GLobal counter at end:",counter)
```
## Example Output :
```
Global counter: 1
Local counter: 1
Nonlocal counter: 1
Outer counter after inner: 1
GLobal counter at end: 1
```
