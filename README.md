import random

def check():
    if comp == user:
        return 0 
    if comp == 0 and user == 2:
        return -1
    if comp == 1 and user == 0:
        return -1
    if comp == 2 and user == 1:
        return -1
    
    else:
        1

print(">>>>>>>>>>>>>>>>>>>>> Welcome to Rock Paper and Scissor game <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<")

comp = random.randint(0,2)
# while user:
#     if(user>3):
#         break
user = int(input("0 is Rock, 1 is for paper, 2 is for scissor \n Enter the number : "))


print(f"comp choosen : {comp}")
print(f"user choosen : {user}")


score = check()
if score == 0:
    print("It's a draw !!")
    print("Play again")
elif score == -1:
    print("You loose!!")
    print("Play again")
elif score == 1:
    print("Congratulations!! You won ")
    print("Play again")
else:
    print(" Opps!! choose number between 0 to 2")
