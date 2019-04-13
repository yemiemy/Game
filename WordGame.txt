import random
print("Let's play a game.")
print("You will try to guess the word I have.")
print("This game helps you work on your guesses")
with open ("/Users/Yemi/Desktop/website/words.txt") as wordList:
    guessWord = random.choice(wordList.readlines()).strip()
    print(guessWord)

while True:
        guess = input("Guess A word")
        if guess == guessWord:
            print ("Bravo! You are great.")
        else:
            print("Oops! Try again.")