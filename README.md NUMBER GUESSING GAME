''' EXPECTED OUTPUT:- Welcome to the Number Guessing Game!
I'm thinking of a number between 1 and 100.
Enter your guess: 50
Too high! Try again.
Enter your guess: 30
Too low! Try again.
Enter your guess: 40
Too low! Try again.
Enter your guess: 45
Too high! Try again.
Enter your guess: 42
Congratulations! You've guessed the number 42 in 5 attempts.
'''
import random

def number_guessing_game():
    print("Welcome to the Number Guessing Game!")
    print("I'm thinking of a number between 1 and 100.")
    
    # Randomly select a number between 1 and 100
    secret_number = random.randint(1, 100)
    
    # Initialize variables
    attempts = 0
    guessed = False
    
    # Start the game loop
    while not guessed:
        # Get the user's guess
        try:
            guess = int(input("Enter your guess: "))
            attempts += 1  # Increment attempt count
            
            # Check if the guess is correct, too high, or too low
            if guess < secret_number:
                print("Too low! Try again.")
            elif guess > secret_number:
                print("Too high! Try again.")
            else:
                print(f"Congratulations! You've guessed the number {secret_number} in {attempts} attempts.")
                guessed = True  # End the loop if the guess is correct
        except ValueError:
            print("Please enter a valid number.")
    
# Start the game
if __name__ == "__main__":
    number_guessing_game()
