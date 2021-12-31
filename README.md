# Operationsonnumbers
Gets only even numbers and performs addition and division on them

#to get three no.s from the user, multiply the first two no. and divide by the 3rd\
#TO ALLOW ONLY EVEN NUMBERS
def checkeven(number):
    for i in range(3):
        if(number % 2 != 0) :
            print("Enter even number")
            number=int((input()))
            continue
        else:
            print("The number is even")
            break
    return number

        #to get first three numbers
print("you have 3 chances else the same number will be taken")
firstno=int(input("enter the first number: "))
firstnumber=checkeven(firstno)
print("the first number is:",firstnumber)
secondno=int(input("enter the second number: "))
secondnumber=checkeven(secondno)
print("the sceond number is",secondnumber)

#addition of two numbers
result_of_addition=int(firstnumber+secondnumber)  #addition of two numbers
print("the result of addition of first two number is:",result_of_addition)

#getting the third number
thirdno=int(input("enter the third number: "))
thirdnumber=checkeven(thirdno)
print("the third number is",thirdnumber)

#final answer
final_answer=int(result_of_addition//thirdnumber) #division
print("The result of division of the result by the third number is:",final_answer)
