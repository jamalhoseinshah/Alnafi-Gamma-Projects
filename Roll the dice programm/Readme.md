

 
"""
##################### ROLL THE DICE ###################
How it works
This is a classic "roll the dice" programme. 
We will be using the random module for this,since we want to randomize the numberswe get from the dice. 
We set two variables (min and max) , lowest and highest number of the dice. 
We then use a while loop, so that the user can roll the dice again. 
The roll_again can be set to any value, but here it's set to "yes" or "y", 
but you can also add other variations to it. 
Rolling the dice
import random
min = 1
max = 6
roll_again = "yes"
while roll_again == "yes" or roll_again == "y":
    print "Rolling the dices..."
    print "The values are...."
    print random.randint(min, max)
    print random.randint(min, max)
    roll_again = raw_input("Roll the dices again?")
    
######################################################
"""

import random

start = input('Please press ENTER to roll the dice.')

def dice():
    dice = random.randint(1,6)
    return dice

print('The number rolled is ',dice(),'.')

while True:
    roll_again = input('Would you like to roll again? Y/N ')

    if roll_again.lower()=="y":
        print('The new number rolled is ',dice(),'.')
    else:
        print('Thanks for playing.')
        break
        
####################### OUTPUT ####################################
Please press ENTER to roll the dice.
The number rolled is  4 .

Would you like to roll again? Y/N y
The new number rolled is  3 .

Would you like to roll again? Y/N n
Thanks for playing.
