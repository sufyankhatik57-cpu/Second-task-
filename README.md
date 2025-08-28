# Second-task-
Create a guessing game
[28/08, 11:55 am] Sufiyan Khatik: import random

def guessing_game():
    number_to_guess = random.randint(1, 100)
    attempts = 0
    print("🎮 Welcome to the Number Guessing Game!")
    print("I'm thinking of a number between 1 and 100.")

    while True:
        try:
            guess = int(input("🔢 Enter your guess: "))
            attempts += 1
            
            if guess < number_to_guess:
                print("📉 Too low. Try again.")
            elif guess > number_to_guess:
                print("📈 Too high. Try again.")
            else:
                print(f"🎉 Correct! You guessed the number {number_to_guess} in {attempts} attempts.")
                break
        except ValueError:
            print("❌ Please enter a valid number.")

# Run the game
guessing_game()
[28/08, 11:55 am] Sufiyan Khatik: 🎮 Welcome to the Number Guessing Game!
I'm thinking of a number between 1 and 100.
🔢 Enter your guess: 50
📉 Too low. Try again.
🔢 Enter your guess: 75
📈 Too high. Try again.
🔢 Enter your guess: 62
📉 Too low. Try again.
🔢 Enter your guess: 70
🎉 Correct! You guessed the number 70 in 4 attempts.
