import random
import string

def generate_password(length=12):
    # Characters to choose from
    characters = string.ascii_letters + string.digits + string.punctuation
    
    # Generate a random password
    password = ''.join(random.choice(characters) for _ in range(length))
    return password

# Ask user for password length
try:
    length = int(input("Enter the desired password length: "))
    if length < 4:
        print("Password length should be at least 4 characters.")
    else:
        print("Generated Password:", generate_password(length))
except ValueError:
    print("Please enter a valid number!")
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
