# Treasure-Island
A fun treasure finding game 
Line of codes :-
print(r'''
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\ ` . "-._ /_______________|_______
|                   | |o ;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/_____ /
*******************************************************************************
''')
print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.")
option1 = input("You are at a cross road. Where would you like to go?"
                  "\nType 'Left' or 'Right'.\n"). lower()

if  option1== "left":
    option2 = input("You've reached a river shore. "
                 "There is an Island on the other side of the river. "
                 "\nType 'Swim' if you would like to swim across the river. "
                 "Type 'Wait' to wait for a boat.\n"). lower()
    if option2 == "wait":
        option3 = input("You've arrived at the Island peacefully. "
                     "Now there is a Mansion with 3 doors. "
                     "\nOne Red, One Yellow & One Blue. Which one would you choose?\n"). lower()
        if option3 == "red":
            print("You fell into the Lava. Game Over.")
        elif option3 == "blue":
            print("You fell into an ice cold lake. Game Over.")
        elif option3 == "yellow":
            print("Congratulations! You've found the precious treasure.")
        else:
            print("The door you chose doesn't exist. Game Over.")
    else:
        print("You have been consumed by Crocodiles. rightGame Over.")
else:
    print("You fell into a quicksand. Game Over.")
