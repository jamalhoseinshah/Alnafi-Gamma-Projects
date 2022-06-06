

 
"""

####################### EXCERCISE NO: 9 #####################################
Guessing Game One

Generate a random number between 1 and 9 (including 1 and 9). Ask the user to guess the number, then tell them whether they guessed too low, too high, or exactly right.


Extras:

Keep the game going until the user types “exit”
Keep track of how many guesses the user has taken, and when the game ends, print this out.
"""
################## SOLUTION #############################################

import random

number = random.randrange(1, 10)
guess = 0
count = 0

while guess != number and guess != "exit":
    guess = input("Please guess a number between 1 and 9. When you want to end the game print 'exit': ")

    if guess == "exit":
        print("Game Over")
        break

    guess = int(guess)
    count += 1
    if guess not in range(1, 10):
        print("You have to guess a number between 1 and 9!")
    elif guess < number:
        print("You've guessed too low!")
    elif guess > number:
        print("You've guessed too high!")
    else:
        if count == 1:
            print("You rock! You've got it at the first try!")
        elif count <= 3:
            print("Well done! You've got it in just {} tries".format(count))
        elif count > 3:
            print("You've got it! It took you {} tries!".format(count))
            
  ######################## OUTPUT ########################################

Please guess a number between 1 and 9. When you want to end the game print 'exit': 4
You've guessed too low!

Please guess a number between 1 and 9. When you want to end the game print 'exit': exit
Game Over

Please guess a number between 1 and 9. When you want to end the game print 'exit': 8
You rock! You've got it at the first try!
            
