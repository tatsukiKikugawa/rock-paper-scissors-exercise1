#game.py
#print("Rock, Paper, Scissors, Shoot!")

import random

print("-------------------")
print("Welcome to my Rock-Paper-Scissors game...")
print("-------------------")

#Processing  user inputs.
#Validating user imputs.
#Simulating computer selection
#Determining the winner
#Displaying results

user_input = input("Please choose either 'rock', 'paper', or 'scissors': ")
if user_input == "rock":
    print("You chose: 'rock' ")
elif user_input == "paper":
    print("You chose: 'paper' ")
elif user_input == "scissors":     
    print("You chose: 'scissors' ")
else:
    exit()

pc_options = ['rock,' 'paper,' 'scissors']
random.choices(pc_options)
print(f"The computer chose: " + str(pc_options) + "!")

print("-------------------")
print("Oh, ")
print("-------------------")
print("Thanks for playing. Pleae play again!")


#-------------------
#Welcome to my Rock-Paper-Scissors game...
#-------------------
#Please choose either 'rock', 'paper', or 'scissors': rock
#You chose: 'rock'
#The computer chose: 'paper'
#-------------------
#Oh, the computer won. It's ok.
#-------------------
#Thanks for playing. Please play again!
