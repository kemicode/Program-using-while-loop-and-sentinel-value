# Program-using-while-loop-and-sentinel-value
#write a program names program44.py that can be used to determine the average of some integers.
#use a while loop and a sentinel value of zero to cease intger input
#display the average to two decimal places
#Pseudocode

#Start Program
#Set Sentinel to 0
#define variable "integer"
#using while loop prompt user to enter an integer or 0 to quit
#set condition if user enters sentinel value the program outputs average
#else output user did not enter any integer
#else output average
#End Program


#Start Program

#Set Sentinel to 0
SENTINEL = 0

#define variable "integer"
integer = []

#using while loop prompt user to enter an integer or 0 to quit
while True:
    number = int(input("Enter integer (0 to quit): "))
#set condition if user enters sentinel value the program outputs average
    if number == SENTINEL:
        break
    integer.append(number)
#else output user did not enter any integer
if not integer:
    print("You didn't enter any integer.")
else:
#else output average
    avg = sum(integer)/len(integer)
    print("average of ", len(integer), " integers is :", avg)

#End of Program
