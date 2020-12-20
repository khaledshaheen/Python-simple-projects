# Python-simple-projects

#Random password generator
from random import randint
#Define a function that returns a random password
def passwordGen():
    MinChar=8
    MaxChar=10
    #random length of the password
    random_lenght=randint(MinChar,MaxChar)
    password=""
    #loop over the length 
    for x in range(random_lenght):

        # add a random letter,special character,number
        password+=chr(randint(33,126))
    return password
def main():
    print("Your random password is:",passwordGen())
main()
