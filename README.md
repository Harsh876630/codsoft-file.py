import math
print("s calculator")
print("1. addition")
print("2. subtraction")
print("3. multiplication")
print("4. division")
print("5. modulus")
print("6. exit")
# Take user choice
choice = input("enter the number(1 to 6):")
#Take action depend on choice
if choice == "1":
    a = float(input("Enter first number: "))
    b = float(input("Enter second number: "))
    print("Result:", a + b)
elif choice =="2":
    a = float(input("Enter first number: "))
    b = float(input("Enter second number: "))
    print("Result:", a - b)
elif choice =="3":
    a = float(input("Enter first number: "))
    b = float(input("Enter second number: "))
    print("Result:", a*b)
elif choice =="4":
    a = float(input("Enter first number: "))
    b = float(input("Enter second number: "))
    print("Result:", a/b)
elif choice =="5":
    a = float(input("Enter first number: "))
    b = float(input("Enter second number: "))
    print("Result:", a%b)
else:
    print("Invalid choice.Please try again")
