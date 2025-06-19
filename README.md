# Python_calculator
def sum(num1,num2):
    return(num1+num2)
def subtraction(num1,num2):
    return(num1-num2)
def Multiplication(num1,num2):
    return(num1*num2)
def Division(num1,num2):
    return(num1/num2)

def calculation():  
    print("Welcome to Basic Calculator\n1.Additioin\n2.Subtraction\n3.Multiplication\n4.Division")
    choice=int(input("Enter number as Shown in above Index."))

    if choice in (1,2,3,4):
        num1=float(input("Enter 1st Number:"))
        num2=float(input("Enter 2nd Number:"))
        if choice == 1:
            print(num1 ,"+",num2,"=", sum(num1,num2))
        elif choice == 2:
            print(num1 ,"-",num2,"=",subtraction(num1,num2))
        elif choice == 3:
            print(num1 ,"*",num2,"=",Multiplication(num1,num2))
        elif choice == 4:
            print(num1 ,"/",num2,"=",Division(num1,num2))
        else:
            print("invalid input !!!\nInput Instruction as given in Index. ")
calculation()



while True:
    repeat=input(("Enter yes for more calculation or no for closing calculation."))
    if repeat.lower() == "yes":
        calculation()
    else:
        print("Thank you for Calculation")
        break
