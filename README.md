# NeuralNetwork_Assignment1

Name : SRINIVAS MUSINURI
UCM Id : 700758813

1.– Input the string “Python” as a list of characters from console, delete at least 2 characters, reversethe
resultant string and print it
/********************************************************************************************/
import random
def main():
    inputString = input("Enter a string: ") 
    if len(inputString) >= 4:
        randomString = random.sample(range(len(inputString)), 2)
        filtered = [c for i, c in enumerate(inputString) if i not in randomString]      
        r = ''.join(reversed(filtered))
        print("Reversed string:", r)

(Took the input string and used python builtin random function to select and remove two random characters in the input, used reversed function to get the reverse string
/********************************************************************************************/


1(b). – Take two numbers from user and perform at least 4 arithmetic operations on them.
/********************************************************************************************/
number1 = float(input("Enter the first number: "))
number2 = float(input("Enter the second number: "))

addition = number1 + number2
subtraction = number1 - number2
multiplication = number1 * number2
# making sure it is not zero here, in avoiding undefined
if number2 != 0:
    division = number1 / number2
print(f"Addition: {addition}")
print(f"Subtraction: {subtraction}")
print(f"Multiplication: {multiplication}")
print(f"Division: {division}")
/********************************************************************************************/

2. Write a program that accepts a sentence and replace each occurrence of ‘python’ with ‘pythons’.
/********************************************************************************************/
inputString = input("Enter the input: ")
modifiedString = inputString.replace('python', 'pythons')
print(modifiedString)
/********************************************************************************************/


3. Use the if statement conditions to write a program to print the letter grade based on an input class score. Use the
grading scheme we are using in this class.
/********************************************************************************************/
inputScore = float(input("Enter the class score: "))
# Given Grading on some estimation, as i dont remember exactly
TopScore = 85
ModerateScore = 70
AverageScore = 60
LowScore = 50

if inputScore >= TopScore:
    letter_grade = "A"
elif inputScore >= ModerateScore:
    letter_grade = "B"
elif inputScore >= AverageScore:
    letter_grade = "C"
elif inputScore >= LowScore:
    letter_grade = "D"
else:
    letter_grade = "F"

print("Student Grade", letter_grade)
/********************************************************************************************/


