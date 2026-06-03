# guess-the-number
#the project uses python code to make a small game in which you can guess the number in between 1 to 100 and the system will tell you if you have guessed it right or wrong.
import random

num= random.randint(1,100)

while True:
    userchoise =(input("guess the number or quit:(Q)"))
    if(userchoise == "Q"):
        break
    
    
    userchoise = int(userchoise)
    if (userchoise == num):
        print("success you won the game")
        break

    elif(userchoise<num):
        print("guess again the number is bigger")

    else:
        print("oo no the number is smaller")

print("Game over....")
