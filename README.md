# Number-Guessing-Game
Number Guessing Game by using the python programming language .

import random

select = (input("Select the mode !\nAuto \Manually .\n"))

if select == "Auto" :
    random_number = random.randint(1,10)
    print("Guess the number between the 1 to 10 .\n")
    guess = 0
    while guess != random_number :
        user_input_number = (int(input("Guess the number : ")))
        print(f"You are entered the number : {user_input_number}\n")
        if user_input_number == random_number :
            print("You Win !\n")
        elif random_number == random_number :
            print(f"You Lost !\nThe number is : {random_number}\nTry Again !\n")
        else :
            print("Something Is wrong Try Again !\n")

if select == "Manually" :
    print("For Manually Mode , Set the starting point and ending point of an number !\n")
    starting_number = int(input("Set the starting point of an number guessing game : "))
    ending_number = int(input("Set the ending point of an number guessing game : "))
    combine_number = random.randint(starting_number,ending_number)
    guess = "XYZ"
    while guess != combine_number :
        user_input_number = (int(input("Guess the number : ")))
        print(f"You are entered the number : {user_input_number}")
        if user_input_number == combine_number :
            print("You Win !")
        elif combine_number == combine_number :
            print(f"You Lost !\nThe number is : {combine_number}\nTry Again !\n")
        else :
            print("Something Is wrong Try Again !\n")
            print("Something Is wrong Try Again !\n")
