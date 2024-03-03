# CODSOFT
# define a simple calculator with arithmetic operations.
n1=int(input("Enter 1st number"))
n2=int(input("Enter 2nd number"))
print("=====Simple Calculator===========")
print("\t 1. Addition")
print("\t 2. Subtraction")
print("\t 3. Multiplication")
print("\t 4. Division")
print("\t 5. modulo")
choice=int(input('Enter your choice between -(1 to 5):'))
if choice==1:
    print(n1+n2)
elif choice==2:
    print(n1-n2)
elif choice==3:
    print(n1*n2)
elif choice==4:
    print(n1/n2)
elif choice==5:
        print(n1%n2)
else:
    print('Invalid choice try again......!')

# Rock-Paper-Scissors Game
print("=====rock paper scissor===========")
print("\t 1. rock")
print("\t 2. paper")
print("\t 3. scissor")
import random
computer_selection=random.randint(1,3)
print(computer_selection)
while(True):
    user_input=int(input('Enter your choice between -(1 to 3):'))
    if (user_input==1 and computer_selection==1) or (user_input==2 and computer_selection==2) or (user_input==3 and computer_selection==3):
        print("no one wins")
    elif (user_input==1 and computer_selection==2) or (user_input==2 and computer_selection==3) or (user_input==3 and computer_selection==1):
        print("computer_selection wins")
    elif (user_input==1 and computer_selection==3) or (user_input==2 and computer_selection==1) or (user_input==3 and computer_selection==2):
        print("user_input wins")
    print("\t Do you want to play again")
    print("\t 1. yes")
    print("\t 2. No")
    choice=int(input('Enter your choice between -(1 to 2):'))
    if choice==2:
       break
    else:
        print("Invalid choice")

# PASSWORD GENERATOR
import string
import random
length = int(input("Enter password length: "))
print("\t 1. characters")
print("\t 2. numbers")
print("\t 3. special_symbols")
print("\t 4. exit")
characterList = ""
while(True):
	choice = int(input("Pick a number "))
	if(choice == 1):
	    characterList=characterList+string.ascii_letters
	elif(choice == 2):
	    characterList=characterList+string.digits
	elif(choice == 3):
	    characterList=characterList+string.punctuation
	elif(choice == 4):
		break
	else:
		print("Please pick a valid option!")
password = []
for i in range(length):
    randomchar = random.choice(characterList)
    password.append(randomchar)
print("The random password is " + "".join(password))

# Contact Book


    
