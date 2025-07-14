# Compound Interest with Loops

# Get the Original Deposit
while True:
    try:
        deposit = float(input("What is the Original Deposit (positive value): "))
        if deposit <= 0:
            print("Input must a positive numeric value")
        else:
            break
    except:
        print("Input must a positive numeric value")

# Get the Interest Rate
while True:
    try:
        interest_rate = float(input("What is the Interest Rate (positive value): "))
        if interest_rate <= 0:
            print("Input must a positive numeric value")
        else:
            break
    except:
        print("Input must a positive numeric value")

# Get the Number of Months
while True:
    try:
        months = int(input("What is the Number of Months (positive value): "))
        if months <= 0:
            print("Input must a positive numeric value")
        else:
            break
    except:
        print("Input must a positive numeric value")

# Get the Goal Amount
while True:
    try:
        goal = float(input("What is the Goal Amount (can enter 0 but not negative)): "))
        if goal < 0:
            print("Input must 0 or greater")
        else:
            break
    except:
        print("Input must 0 or greater")

# Calculate monthly interest rate
monthly_rate = (interest_rate / 100) / 12

# Start account balance
balance = deposit

# Loop for each month to show account balance
for month in range(1, months + 1):
    interest = balance * monthly_rate
    balance = balance + interest
    print(f"Month: {month}  Account Balance is: $ {balance:,.2f}")

# Predict how many months to reach the goal
if goal > deposit:
    balance = deposit
    month_count = 0
    while balance < goal:
        interest = balance * monthly_rate
        balance = balance + interest
        month_count += 1
    print(f"It will take: {month_count:,} months to reach the goal of $ {goal:,.2f}")
