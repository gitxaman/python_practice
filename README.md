import random 
alphabet_to_guess = random.randint(97, 122)  # ASCII values for 'a' to 'z'

while True:
    try:
        
        guess = ord(input("Guess a letter between a and z:"))  # Convert character to ASCII value
        if guess > alphabet_to_guess:
            print("too high!")
        elif guess < alphabet_to_guess:
            print("too low!")
        elif guess == alphabet_to_guess:
            print("congo you guessed it right!")
            break
    except ValueError:
        print("enter a valid letter")   
        
