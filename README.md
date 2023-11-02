A simple calcualtor that has Addition, Subtraction, MUltiplication, and Division.

~ CODE BELOW ~

def calculate(a, b, op):
    if op == "+":
        result = a + b
    elif op == "-":
        result = a - b
    elif op == "*":
        result = a * b
    elif op == "/":
        if b == 0:
            result = "ERROR - CANNOT DIVIDE BY ZERO"
        else:
            result = a / b
    else:
        result = "ERROR - OPERATOR NOT VALID"
    return result

op = input("Operator +, -, *, /: ")
if op in ("+", "-", "*", "/"):
    num1 = float(input("Enter a Number: "))
    num2 = float(input("Enter Another Number: "))
    result = calculate(num1, num2, op)
    print("Result:", result)
else:
    print("ERROR - OPERATOR IS NOT VALID")
