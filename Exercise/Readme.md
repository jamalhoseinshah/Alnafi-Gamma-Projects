"""
################ Exercise 2 ######################################

Ask the user for a number. Depending on whether the number is even or odd, print out an appropriate message to the user.

Hint: how does an even / odd number react differently when divided by 2?

Extras:

If the number is a multiple of 4, print out a different message.
Ask the user for two numbers: one number to check (call it num) and one number to divide by (check). If check divides evenly into num, tell that to the user. 
If not, print a different appropriate message.
#################### SOLUTION ################################

num = input("Enter a number: ")

x = 1 % 2

if x  > 0:
    print("You picked an odd number.")
else:
    print("You picked an even number.")
    
######################## OUTPUT ###################################    

# EXAMPLE NO:1

Enter a number: 13
You picked an odd number.

# EXAMPLE NO:2

Enter a number: 14
You picked an odd number.



################# SECOND EXAMPLE ##########################    
num = int(input("give me a number to check: "))
check = int(input("give me a number to divide by: "))

if num % 4 == 0:
    print(num, "is a multiple of 4")
elif num % 2 == 0:
    print(num, "is an even number")
else:
    print(num, "is an odd number")

if num % check == 0:
    print(num, "divides evenly by", check)
else:
    print(num, "does not divide evenly by", check) 
   
######################## OUTPUT #########################

# EXAMPLE NO: 1
give me a number to check: 12

give me a number to divide by: 3
12 is a multiple of 4
12 divides evenly by 3

# EXAMPLE NO: 2

give me a number to check: 7

give me a number to divide by: 3
7 is an odd number
7 does not divide evenly by 3
    
