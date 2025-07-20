import random

print("Welcome in game Stone, Paper, Scissor!")
print("1. Rock")
print("2. Paper")
print("3. Scissor")
print("4. Rock beats Scissor")
print("5. Paper beats Rock")
print("6. Scissor beats Paper")
print("7. Exit anytime from the game\n")

choices = {
    "1": "rock",
    "2": "paper",
    "3": "scissor"
}

while True:
    choice = input("Enter a number (1 to 3 or 7): ")

    if choice == "7":
        print("You chose to exit the game. Thanks for playing!")
        break

    if choice not in choices:
        print("Invalid input. Please enter 1, 2, 3, or 7.")
        continue

    user_choice = choices[choice]
    computer_choice = random.choice(["rock", "paper", "scissor"])

    print(f"You chose: {user_choice}")
    print(f"Computer chose: {computer_choice}")

    if user_choice == computer_choice:
        print("It's a tie!")
    elif (user_choice == "rock" and computer_choice == "scissor") or \
         (user_choice == "scissor" and computer_choice == "paper") or \
         (user_choice == "paper" and computer_choice == "rock"):
        print("You Win!")
    else:
        print("Computer Wins!")
