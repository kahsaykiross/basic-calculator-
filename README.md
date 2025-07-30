# basic-calculator-
# plp assignment  calculates by accepting two numerical values from user and report error 
# Basic Calculator Program 🧮

# Get input from the user
num1 = float(input("Enter the first number: "))
operator = input("Enter an operation (+, -, *, /): ")
num2 = float(input("Enter the second number: "))

# Perform the calculation
if operator == '+':
    result = num1 + num2
    print(f"{num1} + {num2} = {result}")
elif operator == '-':
    result = num1 - num2
    print(f"{num1} - {num2} = {result}")
elif operator == '*':
    result = num1 * num2
    print(f"{num1} * {num2} = {result}")
elif operator == '/':
    if num2 != 0:
        result = num1 / num2
        print(f"{num1} / {num2} = {result}")
    else:
        print("⚠️ Error: Cannot divide by zero.")
else:
    print("❌ Invalid operator! Please use +, -, *, or /.")
