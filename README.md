# <h1 align="center"><font color='blue'>PYTHON PROGRAMMING ASSIGNMENT</font></h1>
### <h1 align="center"><font color='orange'>Coding Exercises</h1>
Exercise 1: Prime Numbers
<br/>
Write a Python program that checks whether a given number is prime or not. A prime number is a natural number greater than 1 that has no positive divisors other than 1 and itself.
<br/>
```ruby
num = 3
if num > 1:
    for i in range(2, (num//2)+1):
        if (num % i) == 0:
            print(num, "is not a prime number")
            break
    else:
        print(num, "is a prime number")
else:
    print(num, "is not a prime number")
```
3 is a prime number
<br/>

Exercise 2: Product of Random Numbers
<br/>
Develop a Python program that generates two random numbers and asks the user to enter the product of these numbers. The program should then check if the user's answer is correct and display an appropriate message.
<br/>
```ruby
import random

def random_product():
    # Generate two random numbers between 1 and 10
    num1 = random.randint(1, 10)
    num2 = random.randint(1, 10)

    # Calculate the correct product
    correct_answer = num1 * num2

    # Ask the user for their answer
    user_answer = int(input(f"What is the product of {num1} and {num2}? "))

    # Check if the user's answer is correct and display the appropriate message
    if user_answer == correct_answer:
        print("Correct! Well done!")
    else:
        print(f"Incorrect. The correct answer is {correct_answer}.")

#Run the random_product
random_product()
```
