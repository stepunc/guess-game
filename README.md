# guess-game
import random
random_number = random.randint(1,100)
guess = -1

while guess != random_number:
    try:
        guess = int(input(" Enter a guess between 1 and 100: "))
        if  guess < random_number:
            print(" too low. please pick again")
        elif guess > random_number:
            print(" too high. Plaese pick again")
        else: 
            print(" Congratulations! you guessed correctly!")
    except ValueError:
         print("Invalid input! Please enter a valid integer.")
