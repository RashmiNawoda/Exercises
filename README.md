# Exercises
#python Exercises 
#this included simple python programme.
"""The game is played by Dealerand Player. Dealergenerates a randominteger number between 0 and 10. Player has to guess it. The program should take input from Player as long as Player inputs same numberas Dealer’s input was. Player getsadviceto choose greater or smaller numbers in next choice.Finally,program has to also displaythe number of tries until the number is guessed and program to allow second play where another player can play and finally also display fi Player1 or Player2 wins, by comparing the numbers of tries and choosing the one with smaller number."""

import random
Guess_1 =0
No_Of_Guesses_1 = 0
No_To_Guess_1 =  random.randint(0, 10)
while Guess_1 != No_To_Guess_1 and No_Of_Guesses_1 <10 :
    Guess_1 = int(input("Player1 : "))
    No_Of_Guesses_1 = No_Of_Guesses_1 + 1
    if Guess_1 == No_To_Guess_1:
         print("That's Right. Number of tries",No_Of_Guesses_1,"\n",)
    else :
        if (Guess_1 > No_To_Guess_1):
            print("Try a Smaller Number")
        else :
            print("Try a Greater Number")
 
Guess_2 = 0
No_Of_Guesses_2 = 0
No_To_Guess_2 =  random.randint(0, 10)
while Guess_2 != No_To_Guess_2 and No_Of_Guesses_2 <10 :
    Guess_2 = int(input("Player2 : "))
    No_Of_Guesses_2 = No_Of_Guesses_2 + 1
    if Guess_2 == No_To_Guess_2:
         print("That's Right. Number of tries",No_Of_Guesses_2,"\n",)
    else :
        if (Guess_2 > No_To_Guess_2):
            print("Try a Smaller Number")
        else :
            print("Try a Greater Number")
            
if (No_Of_Guesses_1 < No_Of_Guesses_2):
    print("Winner is player1")
else:
    print("Winner is player2")   
