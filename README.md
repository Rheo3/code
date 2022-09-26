# code
simple rock paper scissors
print('simple rock paper scissors')
import random
user_action = input("enter a choice{rock,paper, scissors}:")
possible_actions = ["rock","paper","scissors"]
computer_action = random.choice(possible_actions)

print(f"\nyou chose {user_action}, computer chose {computer_action}.\n")

if user_action == computer_action:
    print(f"Both players selected {user_action}. It's a tie!")
elif user_action == "rock":
    if computer_action == "scissors":
        print("Rock wins over scissors You win!")
    else:
        print("Paper wins over rock You lose.")
elif user_action == "paper":
    if computer_action == "rock":
        print("Paper wins rock You win!")
    else:
        print("Scissors wins over paper You lose.")
elif user_action == "scissors":
    if computer_action == "paper":
        print("Scissors wins over paper You win!")
    else:
        print("Rock wins over scissors You lose.")
