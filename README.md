# guess-_the-_number
# guess the number
import random

target = random.randint(1,100)

while True:
    userChoice = input("guess the target or quit(Q): ")
    if(userChoice == "Q"):
        break
    userChoice = int(userChoice)
    if(userChoice == target):
        print("success : correct guess!!")
        break
    elif(userChoice < target):
        print("your number was too small. take a bigger  guess...")
    else:
        print("your number was too big. take a smaller guess...")


print("------Game over-----")    
