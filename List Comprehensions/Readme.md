


"""
###################   Exercise 7  ##############################################

List comprehensions

Let’s say I give you a list saved in a variable: a = [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]. Write one line of Python that takes this list a and makes 
a new list that has only the even elements of this list in it.
"""

################# SOLUTION ############################################


# Python program to print even Numbers in a List
 
# list of numbers
a = [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
 
# using list comprehension
even_nos = [num for num in a if num % 2 == 0]
 
print("Even numbers in the list: ", even_nos)


#################### OUTPUT ###################################

Even numbers in the list:  [4, 16, 36, 64, 100]
