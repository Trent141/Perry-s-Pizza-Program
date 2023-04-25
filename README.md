# Perry-s-Pizza-Program
#I am creating a small program that calculates the charge behind a pizza order, unfortunately I am having problems with the program as it doesn't calculate correctly.  
#I also need to implement a GUI


print("Welcome to Perry's Pizza. What would you like today? ")
size = input("What size pizza Would you like? S, M, or L: ")
addpep = input("Would you like pepperoni? Y or N: ")
extchse = input("Would you like extra cheese? Y or N: ")
bredstcks = input("Would you like Breadsticks ? Y or N: ")

bill = 0

if size == "S":
    bill += 15
elif size == "M":
    bill += 20
elif size == "L":
    bill += 25

if addpep == "Y":
    if size == "S":
        bill += 2
    else:
        bill += 3
        
if extchse == "Y":
    bill += 1

if bredstcks == "Y":
    bill += 2

    
print(f"Your total is {bill}") 
