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
What is the product of 4 and 9? 78
<br/>
Incorrect. The correct answer is 36.
<br/>

Exercise 3: Squares of Even/Odd Numbers
<br/>
Create a Python script that prints the squares of all even or odd numbers within the range of 100 to 200. Choose either even or odd numbers and document your choice in the code.
<br/>
```ruby
def print_squares():
    # Loop through the range 100 to 200
    for number in range(100, 201):
        # Check if the number is even
        if number % 2 == 0:
            # Print the square of the even number
            print(f"The square of {number} is {number ** 2}")

# Run the function
print_squares()
```
The square of 100 is 10000
The square of 102 is 10404
The square of 104 is 10816
The square of 106 is 11236
The square of 108 is 11664
The square of 110 is 12100
The square of 112 is 12544
The square of 114 is 12996
The square of 116 is 13456
The square of 118 is 13924
The square of 120 is 14400
The square of 122 is 14884
The square of 124 is 15376
The square of 126 is 15876
The square of 128 is 16384
The square of 130 is 16900
The square of 132 is 17424
The square of 134 is 17956
The square of 136 is 18496
The square of 138 is 19044
The square of 140 is 19600
The square of 142 is 20164
The square of 144 is 20736
The square of 146 is 21316
The square of 148 is 21904
...
The square of 194 is 37636
The square of 196 is 38416
The square of 198 is 39204
The square of 200 is 40000
Output is truncated. View as a scrollable element or open in a text editor. Adjust cell output settings...
