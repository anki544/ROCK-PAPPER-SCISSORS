# Game : Rock, paper, scissors 

import random

print("ROCK, paper,Scissors GAME")

options = ["rock","paper","scissors"]

user = input("Enter your choice: ").lower()

computer = random.choice(options)

print("Computer: ", computer)

# Tie case 
if user == computer:
    print("It is a Tie")

# Your win cases
elif user == "rock" and computer == "scissors":
    print("You win")
elif user == "paper" and computer == "rock":
    print("You win")
elif user == "scissors" and computer == "paper":
    print("You win")

# Computer win cases 
elif user == "scissors" and computer == "rock":
    print("Computer win")
elif user == "rock" and computer == "paper":
    print("Computer win")
elif user == "paper" and computer == "scissors":
    print("Computer win")

# invalid case 
else:
    print("Invalid input")
