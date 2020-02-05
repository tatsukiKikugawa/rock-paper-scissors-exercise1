#game.py
#print("Rock, Paper, Scissors, Shoot!")

import random

print("-------------------")
print("Welcome to my Rock-Paper-Scissors game...")
print("-------------------")

#Processing  user inputs.
x = input("Please choose either 'rock', 'paper', or 'scissors':  ")
print(f"You chose: " + str(x))

#Validating user imputs.
user_choice = ["rock", "paper", "scissors"]
if x in user_choice:
    print("VALID")
else:
    print("INVALID")
    exit()

#Simulating computer selection

pc_choice = random.choices(user_choice)
pc_choice = ",".join(pc_choice) #Use ",".join(variable) to convert a list item to a string
print(f"The computer chose: " + str(pc_choice) + "!")

#Determining the winner
pc_choice = pc_choice.lower()
x = x.lower()

print(pc_choice)
print(x)

#Displaying results
if pc_choice == x:
    print("TIE")
elif pc_choice == "rock":
    if x == "scissors":
        print("You lose. Play again!")
    elif x == "paper":
        print("You win. Play again")
elif pc_choice.lower() == "paper":
    if x == "rock":
        print("You lose. Play again!")
    elif x == "scissors":
        print("You win. Play again")
elif pc_choice == "scissors":
    if x == "paper":
        print("You lose. Play again!")
    elif x == "rock":
        print("You win. Play again")
    
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
