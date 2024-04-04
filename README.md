# advanced-calculator-for-older-children-
This calculator code is designed for older children and in more advanced. 
import time

while True: #CREATING A LOOP
    print("\nWELCOME TO YOUR ADVANCED CALCULATOR!\n")
    cont = input("Would you like to use your calculator? y/n:\n").lower() #BASICALLY TURNING THE CALCULATOR ON OR OFF
    if cont == "n":
        break #ENDS PROGRAM

    cont = input("Are you 10 years of age or older? :y/n\n").lower() #THE PROGRAM IS FOR USERS 10 YEAR AND OVER
    if cont == "n":
        print("Then you should try the simple calculator for younger children")#THIS IS NOT A SIMPLE CALCULATOR
        break #ENDS PROGRAM

    time.sleep(2)
    print("Awesome, let me show you some simple mathematics! \n")
    time.sleep(2)
    print("(+) Example of Addition: 1 rabbit + 1 rabbit = 2 rabbits")
    time.sleep(2)
    print("\U0001f407 \U0001f407 \n")
    time.sleep(2)
    print("(-) Example of Subtraction: 10 ducks - 5 ducks = 5 ducks")
    time.sleep(2)
    print("\U0001F986 \U0001F986 \U0001F986 \U0001F986 \U0001F986 \n")
    time.sleep(2)
    print("(*) Example of Multiplication: 3 kittens x 3 kittens = 9 kittens")
    time.sleep(2)
    print("\U0001F431 \U0001F431 \U0001F431 \U0001F431 \U0001F431 \U0001F431 \U0001F431 \U0001F431 \U0001F431 \n")
    time.sleep(2)
    print("(/) Example of Division: 12 eggs / by 2  = 6 eggs remaining")
    time.sleep(2)
    print("\U0001F95A \U0001F95A \U0001F95A \U0001F95A \U0001F95A \U0001F95A \n")
    time.sleep(2)
    print("Let's have some fun with numbers! \n")
    time.sleep(2) #this time delay gives the use more time to follow the functions

    NAME = input("What is your Name?: ") #CONNECTING WITH THE USER
    print("Hi," + NAME)
    user_input = input('Do you want to play a Magic Game (y/n): ').lower()

    if user_input.lower() == 'y':
        print("Fantastic, let the magic begin!\n")

    elif user_input.lower() == "n":
        print("Ok Bye! \n")
        break

    import random
    def calculator_trick():
        secret_number = random.randint(1,20)
        print("Welcome to the Magic Calculator Trick...\n")
        print("Think of a number between 1 and 20.")
        input("Press Enter when ready...\n")
        print("Now, add", secret_number, "to your number.")
        input("Press Enter when ready...\n")
        result = 2 * secret_number
        print("Double the result.")
        input("Press Enter when ready...\n")
        print("Now, subtract the original number you thought of.")
        input("Press Enter when ready...\n")
        print("Congratulations! Your Magic Number is:", result,"\U0001F389 \U0001F389 \U0001F389 \U0001F389 \U0001F389 \n")

    calculator_trick()

    print("Please select the mathematical calculation you want to perform?")  # "User Instruction"
    print("1. for (+) Addition")  # "the 4 mathematical options available"
    print("2. for (-) Subtraction")
    print("3. for (*) Multiplication")
    print("4. for (/) Division")
    print("5. for (%) Percentage on my school test? ")
# "print statements to inform the user"
    operation = input()  # "input to ask the user to respond
    if operation == "1":  # "quotation marks important" #"Is equal to (==)"
        num1 = input("Enter first number:")  # "user instruction"
        num2 = input("Enter second number:")  # "user instruction"
        num3 = input("Enter third number:")  # "extra code"
        print("The sum is: " + str(float(num1) + float(num2) +float(num3)))  # "a string of whole numbers" added third number option

    elif operation == "2": # "could use x, y, z, etc instead of numbers to reflect a variable"
        num1 = input("Enter first number:") #"num1 or num2 could be referred to as x or y"
        num2 = input("Enter second number:")
        num3 = input("Enter third number:")
        print("The difference is: " + str(float(num1) - float(num2) - float(num3)))  # (wk4 I added a float instead on int, "a string of whole numbers only, not sure how to use a float in this line for decimal"

    elif operation == "3":
        num1 = input("Enter first number:")
        num2 = input("Enter second number:")
        num3 = input("Enter third number:")
        print("The sum is: " + str(float(num1) * float(num2) * float(num3))) #(wk4)added a float instead of int and another option for user

    elif operation == "4":
        num1 = input("Enter first number:")
        num2 = input("Enter second number (not 0):")
        num3 = input("Enter third number (not 0):")
        print("The answer is: " + str(float(num1) / float(num2) / float(num3))) #(wk4)added a float instead of int and another option for user

    elif operation == "5":
        num1 = input("How many questions did you answer correct?  ")
        num2 = input("How many questions are on the test sheet? Please enter a number: ")#percentage x whole number divided by 100
        print("Great, your score was:  " + str(float(num1) / float(num2) * float(100)) + " % ") #this is a new function
#i am using a formula to work out a childs test marks, taking their score, deviding it by the total marks and multiplying it by 100 to get a percentage
        print("\U0001F600 \U0001F600 \U0001F600 ")
    else:
        print("Invalid Entry")  # "the code only recognises option 1, 2, 3, 4, 5, or 6"
    #cont = "y"
    #while cont.lower() == "y":
    #print("select operation\n1.Addition\n2.Subtraction\n3.Multiplication\n4.Divide\n5.Percentage")
        if operation == "1":  # "qoutation marks important" #"Is equal to (==)" wk4 I had to insert this code for the loop to work
            num1 = input("Enter first number:")  # "user instruction"
            num2 = input("Enter second number:")  # "user instruction"
            num3 = input("Enter third number:")  # extra code
            print("The sum is: " + str(float(num1) + float(num2) + float(num3)))  # "a string of whole numbers" added third number option

        elif operation == "2":
            num1 = input("Enter first number:")
            num2 = input("Enter second number:")
            num3 = input("Enter third number:")
            print("The difference is: " + str(float(num1) - float(num2) - float(num3)))  # (wk4 I added a float instead on int, "a string of whole numbers only, not sure how to use a float in this line for decimal"

        elif operation == "3":
            num1 = input("Enter first number:")
            num2 = input("Enter second number:")
            num3 = input("Enter third number:")
            print("The sum is: " + str(
                float(num1) * float(num2) * float(num3)))  # (wk4)added a float instead of int and another option for user

        elif operation == "4":
            num1 = input("Enter first number:")
            num2 = input("Enter second number:")
            num3 = input("Enter third number:")
            print("The answer is: " + str(
                float(num1) / float(num2) / float(num3)))  # (wk4)added a float instead of int and another option for user

        elif operation == "5":
            num1 = input("How many questions did you answer correct?  ")
            num2 = input("How many questions are on the test sheet? Please enter a number:")  # percentage x whole number divided by 100
            print("Great, your score was:  " + str(float(num1) / float(num2) * float(100)) + " % ")  # this is a new function
    # i am using a formula to work out a childs test marks, taking their score, deviding it by the total marks and multiplying it by 100 to get a percentage
        #else:
            #print("Invalid Entry")  # "the code only recognises option 1, 2, 3, 4, or 5"

        cont = input("Would you like to continue? y/n:") #give user an option to end the program
        if cont == "n":
            break #this break exits the program
