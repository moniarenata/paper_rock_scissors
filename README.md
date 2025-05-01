# paper_rock_scissors
An easy game of paper, rock and scissors.

What the Code Does:
A simple Rock-Paper-Scissors game between the user and the computer.

Uses a loop to keep the game running until the user quits.

Tracks and displays how many times the user and computer won.


Code explanation:

import random

Used to let the computer make a random choice between rock, paper, and scissors.

user_wins = 0, computer_wins = 0

Keeps track of the score during the game.

options = ['rock', 'paper', 'scissors']

Stores the valid choices in a list for easier comparison and selection.

while True:

Creates an infinite loop to keep the game running until the user chooses to quit.

input('Type Rock/Paper/Scissors or Q to quit:').lower()

Converts the user’s input to lowercase so the comparison is case-insensitive.

if user_input == 'q': break

Allows the user to exit the game by typing "q".

if user_input not in options: continue

Skips to the next loop if the input isn’t valid, avoiding unnecessary checks or errors.

random.randint(0,2)

Randomly selects a number between 0 and 2 to simulate the computer's move.

computer_guess = options[random_number]

Converts the random number to one of the valid choices.

Win conditions (if user_input == 'rock' and computer_guess == 'scissors', etc.)

Checks if the user has won and updates the score.

else: print('You lost!')

Handles both ties and computer wins in a single block (since ties are treated as losses here).

Final print() statements

Show how many rounds the user and the computer won after quitting the game.
