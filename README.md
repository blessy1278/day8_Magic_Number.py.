# day8_Magic_Number.py.
#If you repeatedly add its digits until you get a single digit, and that digit is 1.
num = int(input("Enter a number: "))

while num > 9:
    total = 0

    while num > 0:
        digit = num % 10
        total = total + digit
        num = num // 10

    num = total

if num == 1:
    print("Magic Number")
else:
    print("Not a Magic Number")
