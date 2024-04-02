# simple game
import random

# Generate a random number between 1 and 100
secret_number = random.randint(1, 100)

print("Welcome to the MUKONESI game!")
print("I'm thinking of a number between 1 and 100.")

# Initialize the number of guesses
num_guesses = 0

while True:
    # Get user's guess
    guess = int(input("Take a guess: "))

    # Increase the number of guesses
    num_guesses += 1

    # Compare the guess with the secret number  
    if guess < secret_number:
        print("Too low!")
    elif guess > secret_number:
        print("Too high!")
    else:
        print("Congratulations! You guessed the number in", num_guesses, "guesses!")
        break
