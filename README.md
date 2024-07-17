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
