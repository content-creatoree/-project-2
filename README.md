# -project-2
def guess_the_number():
    print("Welcome to the Guess the Number Game!")
    print("I'm thinking of a number between 1 and 100. Can you guess it?")

    # Generate a random number between 1 and 100
    number_to_guess = random.randint(1, 100)
    attempts = 0

    while True:
        try:
            # Prompt the user for a guess
            guess = int(input("Enter your guess: "))
            attempts += 1

            if guess < number_to_guess:
                print("Too low! Try again.")
            elif guess > number_to_guess:
                print("Too high! Try again.")
            else:
                print(f"Congratulations! You guessed the number in {attempts} attempts.")
                break
        except ValueError:
            print("Please enter a valid number.")

# Start the game
guess_the_number()
Welcome to the Guess the Number Game!
I'm thinking of a number between 1 and 100. Can you guess it?
Enter your guess: 78
Too low! Try again.
Enter your guess: 99
Too high! Try again.
Enter your guess: 100
Too high! Try again.
Enter your guess: 79
Too low! Try again.
Enter your guess: 
Please enter a valid number.
