## Library Management
## Code :
```
class book():
    def __init__(self,title,author):
        self.title= title
        self.author= author
        self.available= True
        
    def display_info(self):
        availability= "available" if self.available else "not available"
        print(f"{self.title} by {self.author}- {availability}")        
class library():
    def __init__(self):
        self.books= []
        
    def add_book(self,book):
        self.books.append(book) 
        
    def show_book(self):
        if not self.books:
            print("no book")
        else:
            for book in self.books:
                book.display_info()
                
    def borrow_book(self,title):
        for book in self.books:
            if book.title.lower()== title.lower():
                if book.available:
                    book.available= False
                    print(f"You borrowed {book.title}.")
                else:
                    print(f"{book.title} is already borrowed.")
                return
        print("Book not found")
           
lib= library()
lib.add_book(book("Python Basic","John Doe"))
lib.add_book(book("OOP in Python","Jane Smith"))
lib.add_book(book("Data Science 101","Emily Brown"))
while True:
    print("\n---Library Menu----")
    print("1. Show all Books")      
    print("2 Borrow abook")
    print("3. Exit")
    choice= input("Enter choice:")   
    if choice =="1":
        lib.show_book()
    elif choice == "2":
        title = input("Enter Book title:")
        lib.borrow_book(title)
    elif choice== "3":
        print("Exit")
        break
    else:
        print("Wrong choice")
```
## Example Output :
```
---Library Menu----
1. Show all Books
2 Borrow abook
3. Exit
Enter choice: 1
Python Basic by John Doe- available
OOP in Python by Jane Smith- available
Data Science 101 by Emily Brown- available

---Library Menu----
1. Show all Books
2 Borrow abook
3. Exit
Enter choice: 2
Enter Book title: python basic
You borrowed Python Basic.

---Library Menu----
1. Show all Books
2 Borrow abook
3. Exit
Enter choice: 1
Python Basic by John Doe- not available
OOP in Python by Jane Smith- available
Data Science 101 by Emily Brown- available

---Library Menu----
1. Show all Books
2 Borrow abook
3. Exit
Enter choice: 3
Exit
```



        
        


    
        
    
    

