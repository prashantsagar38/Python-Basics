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
<br/>
The square of 102 is 10404
<br/>
The square of 104 is 10816
<br/>
The square of 106 is 11236
<br/>
The square of 108 is 11664
<br/>
The square of 110 is 12100
<br/>
The square of 112 is 12544
<br/>
The square of 114 is 12996
<br/>
The square of 116 is 13456
<br/>
The square of 118 is 13924
<br/>
The square of 120 is 14400
<br/>
The square of 122 is 14884
<br/>
The square of 124 is 15376
<br/>
The square of 126 is 15876
<br/>
The square of 128 is 16384
<br/>
The square of 130 is 16900
<br/>
The square of 132 is 17424
<br/>
The square of 134 is 17956
<br/>
The square of 136 is 18496
<br/>
The square of 138 is 19044
<br/>
The square of 140 is 19600
<br/>
The square of 142 is 20164
<br/>
The square of 144 is 20736
<br/>
The square of 146 is 21316
<br/>
The square of 148 is 21904
<br/>
...
<br/>
The square of 194 is 37636
<br/>
The square of 196 is 38416
<br/>
The square of 198 is 39204
<br/>
The square of 200 is 40000
<br/>
Output is truncated. View as a scrollable element or open in a text editor. Adjust cell output settings...
<br/>

Exercise 4: Word counter
<br/>
write a program to count the number of words in a given text.
<br/>

```ruby
def count_words(text):
    # Split the text into words using whitespace as the delimiter
    words = text.split()
    # Count the number of words
    num_words = len(words)
    return num_words

# Ask the user to input a text
user_text = input("Enter a text: ")

# Count the number of words in the user's text
word_count = count_words(user_text)

# Display the result
print(f"The number of words in the given text is: {word_count}")
```

<br/>

Enter a text: this world is full of beautiful natural tress and rain drops are increasing because of these trees in the mountains
<br/>
The number of words in the given text is: 20
<br/>

Exercise 5: Check for Palindrome
<br/>
Write a Python function called is_palindrome that takes a string as input and returns True if the string is a palindrome, and False otherwise. A palindrome is a word, 
<br/>
phrase, number, or other sequence of characters that reads the same forward and backward, ignoring spaces, punctuation, and capitalization.
<br/>

```ruby
import string

def is_palindrome(s):
    # Remove spaces and punctuation, and convert to lowercase
    cleaned_string = ''.join(char.lower() for char in s if char.isalnum())

    # Check if the cleaned string is equal to its reverse
    return cleaned_string == cleaned_string[::-1]

# Example usage
example_string = "mom"
print(f"Is the string '{example_string}' a palindrome? {is_palindrome(example_string)}")
```
<br/>

Is the string 'mom' a palindrome? True
