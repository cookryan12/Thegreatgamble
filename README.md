# Thegreatgamble
# This is a Number Guessing Game.
# This is a Number Guessing Game.
import random

print('Hello. What is your name?')

name=input()

print('Well, ' + name +', I am thinking of a number between 1 and 20')

secretnumber = random.randint(1, 20)

for guessestaken in range (1,7):
    
    print('Take a guess.')
    guess=int(input())

    if guess < secretnumber:
        print('Your guess is too low')
    elif guess> secretnumber:
        print('Your guess is too high.')
    else:
        break # this condition is for the correct guess
if guess == secretnumber:
    
    print('Good job! You guessed my number in ' +  str(guessestaken) + ' guesses.')
else:
   
    print('Nope The number I was thinking of was' +  str(secretnumber))















print('You took ' +  str(guessestaken) +  ' guesses.')
