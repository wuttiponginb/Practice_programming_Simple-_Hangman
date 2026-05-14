print("---Simple Hangman---")
import random

word_animal = ("dog", "cat" ,"bird" ,"ant")
word = random.choice(word_animal)
count = 0
while True:
    if count < 6:
        animal = str(input("Which animal do you want guess?: "))
        count += 1
        if animal == word:
            print("---You guessed is correct! %s---"% word )
            print("---You guessed is %d times---"% count)
            break
        else:
            print("---You guessed is wrong!---")
    elif count == 6:
        print("---Game Over!---")
        break
