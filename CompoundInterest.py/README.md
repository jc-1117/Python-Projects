# 1. Ask the user to enter the following:
P = float(input("Enter the starting principle amount: "))

r = float(input("Enter the annual interest rate: "))

n = int(input("How many times per year is the interest compounded? "))

t = int(input("For how many years will the account earn interest? "))

# 2. Convert
P = float(P)
r = float(r) /100
n = int(n)
t = int(t)

# 3. Calculate the amount of money in the account after the given number of years
amount = P * (1 + r / n) ** (n * t)

# 4. Print the final amount
print("At the end of", t, "years you will have ${0:.2f}".format(amount))

