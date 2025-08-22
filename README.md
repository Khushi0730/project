# project
# 1. Add two numbers <br>
a = int(input('Enter any number :  ')) <br>
b = int(input('Enter any number :  '))  <br>
def add_two_numbers(a,b):  <br>
<pre> return a+b </pre>  <br>

# 2. Find the square of a number <br> 
c = int(input('Enter any number: ')) <br>
def square(c): <br>
    return c*c <br>

# 3. Check if a number is even or odd <br> 
num = int(input('Enter any number: ')) <br> 
def even_or_odd(num): <br>
    return "Even" if num % 2 == 0 else 'odd' <br>

# 4. Find the maximum of three numbers <br>
a = int(input('Enter any number :  ')) <br>
b = int(input('Enter any number :  ')) <br>
c = int(input('Enter any number :  ')) <br>
def maximum_of_three(a,b,c): <br>
    return max(a,b,c) <br>

# 5. Calculate factorial of a number <br>
n = int(input('Enter any number:  ')) <br>
def factorial(n): <br> 
    result = 1 <br>
    for i in range(1,n+1): <br> 
        result *= i <br>
    return result <br>

# 6. Count vowels of a string <br>
s = input("Enter a string :  ") <br>
def count_vowels(s): <br>
    vowels = 'aeiouAEIOU'<br>
    count = 0 <br>
    for ch in s: <br>
        if ch in vowels: <br>
            count += 1 <br>
        return count <br>

# 7. Reverse a string <br>
s = input('Enter a string') <br>
def reverse_string(s): <br>
    return s[::-1] <br>

# 8. 

