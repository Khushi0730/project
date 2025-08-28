# project
# 1. Add two numbers <br>
a = int(input('Enter any number :  ')) <br>
b = int(input('Enter any number :  '))  <br>
def add_two_numbers(a,b):  <br>
&nbsp;&nbsp;&nbsp;&nbsp;return a+b   <br>

# 2. Find the square of a number <br> 
c = int(input('Enter any number: ')) <br>
def square(c): <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return c*c <br>

# 3. Check if a number is even or odd <br> 
num = int(input('Enter any number: ')) <br> 
def even_or_odd(num): <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return "Even" if num % 2 == 0 else 'odd' <br>

# 4. Find the maximum of three numbers <br>
a = int(input('Enter any number :  ')) <br>
b = int(input('Enter any number :  ')) <br>
c = int(input('Enter any number :  ')) <br>
def maximum_of_three(a,b,c): <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return max(a,b,c) <br>

# 5. Calculate factorial of a number <br>
n = int(input('Enter any number:  ')) <br>
def factorial(n): <br> 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;result = 1 <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for i in range(1,n+1): <br> 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;result *= i <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return result <br>

# 6. Count vowels of a string <br>
s = input("Enter a string :  ") <br>
def count_vowels(s): <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vowels = 'aeiouAEIOU'<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;count = 0 <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for ch in s: <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if ch in vowels: <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;count += 1 <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return count <br>

# 8. Check if a number is prime <br>
def is_prime(n):
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if n <= 1:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return False
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for i in range(2, int(n**0.5) + 1):
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if n % i == 0:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return False
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return True


# 8. 

