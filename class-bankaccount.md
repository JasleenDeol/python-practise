## Code :
```
class BankAccount:
    def __init__(self,account_holder,balance=0):
        self.account_holder= account_holder
        self.balance= balance
    def deposit(self,amount):
        print(f"Depositing {amount} ...")
        self.balance += amount
        print(f"balance after deposit {self.balance}")
    def withdraw(self,amount):
        print(f"withdrawing {amount}...")
        if self.balance>= amount:
            self.balance -= amount
            print(f"Balance after Withdrawl {self.balance}")
        else:
            print("Insufficient Balance!")
    def display(self):
        print(f"Final Balance= {self.balance}")
p= BankAccount("Alice")

print("Account Holder:", p.account_holder)
print("Initial Balance:", p.balance)

p.deposit(500)

p.withdraw(200)

p.withdraw(500)

p.display()
```
## Output Run :
```
Account Holder: Alice
Initial Balance: 0
Depositing 500 ...
balance after deposit 500
withdrawing 200...
Balance after Withdrawl 300
withdrawing 500...
Insufficient Balance!
Final Balance= 300
```

        
