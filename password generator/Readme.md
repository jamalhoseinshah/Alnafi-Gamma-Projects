

# -*- coding: utf-8 -*-
"""
############################ RANDOM PASSWORD GENERATOR ########################
For this challenge, we will use a Python script to generate a random password
of 8 characters. Each time the program is run, a new password will be generated 
randomly. The passwords generated will be 8 characters long and will have to 
include the following characters in any order:

2 uppercase letters from A to Z,
2 lowercase letters from a to z,
2 digits from 0 to 9,
2 punctuation signs such as !, ?, “, # etc.
To solve this challenge we will have to generate random characters and to do
so we will need to use the ASCII code.
"""

import random
import string
### function for shuffle any string value:
def random_shuffle(string_val):
    temp_string = list(string_val)
#     print(temp_string)
    random.shuffle(temp_string)
    return "".join(temp_string)

def random_paasword_generator():
    uppercaseletter1 =  chr(random.randint(65,90))
    uppercaseletter2 =  chr(random.randint(65,90))
    # print('uppercaseletter2', uppercaseletter2)
    # print('uppercaseletter1', uppercaseletter1)
    lowercaseletter1 = chr(random.randint(98,120))
    lowercaseletter2 = chr(random.randint(98,120))
    # print('lowercaseletter1', lowercaseletter1)
    # print('lowercaseletter2',lowercaseletter2)
    digit1 = random.randint(0,9)
    digit2 = random.randint(0,9)
    # print('digit1', digit1)
    # print('digit2', digit2)
    punctuatuion1 = random.choice(string.punctuation)
    punctuatuion2 = random.choice(string.punctuation)
    # print('punctuatuion1', punctuatuion1)
    # print('punctuatuion2', punctuatuion2)
    password = uppercaseletter1 + uppercaseletter2 + lowercaseletter1 + lowercaseletter2 + str(digit1) + str(digit2) + punctuatuion1 + punctuatuion2
    final_password = random_shuffle(password)
    return final_password

random_paasword_generator()


########################################################## OUTPUT ########################################################################################
# SOME BELOW EXAMPLE AFTER RUN OUR PROGRAMME.

random_paasword_generator()
Out[3]: 'e{;Rj8K6'

random_paasword_generator()
Out[4]: '+G73cxD>'
