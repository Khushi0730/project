<b><i> Basic Function Questions</i></b>

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

# 7. Reverse a string.<br>
def reverse_string(s):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return s[::-1]


# 8. Check if a number is prime <br>
def is_prime(n):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if n <= 1:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return False<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for i in range(2, int(n**0.5) + 1):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if n % i == 0:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return False<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return True<br>


# 9. Calculate simple interest
def simple_interest(principal, rate, time):
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return (principal * rate * time) / 100

# 10. Check if string is palindrome
def is_palindrome(s):
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return s == s[::-1] 

<b><i>Medium Level Function Question</b></i>

# 1. Fibonacci series up to n terms
def fibonacci(n):
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a, b = 0, 1
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;series = []
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for _ in range(n):
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;series.append(a)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a, b = b, a + b
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return series

# 2. GCD of two numbers
def gcd(a, b):
    while b:
        a, b = b, a % b
    return a

# 3. LCM of two numbers
def lcm(a, b):
    return abs(a * b) // gcd(a, b)

# 4. Sum of digits of a number
def sum_of_digits(n):
    return sum(int(digit) for digit in str(abs(n)))

# 5. Second largest element in list
def second_largest(lst):
    unique = list(set(lst))
    unique.sort()
    return unique[-2] if len(unique) >= 2 else None

# 6. Frequency of characters in string
def char_frequency(s):
    freq = {}
    for ch in s:
        freq[ch] = freq.get(ch, 0) + 1
    return freq

# 7. Check if number is Armstrong
def is_armstrong(n):
    digits = str(n)
    power = len(digits)
    return n == sum(int(d) ** power for d in digits)

# 8. Check if number is Perfect
def is_perfect(n):
    if n < 2:
        return False
    divisors = [i for i in range(1, n) if n % i == 0]
    return sum(divisors) == n

# 9. Return sorted list without using sort()
def manual_sort(lst):
    for i in range(len(lst)):
        for j in range(i + 1, len(lst)):
            if lst[i] > lst[j]:
                lst[i], lst[j] = lst[j], lst[i]
    return lst

# 10. Word with maximum length in string
def max_length_word(s):
    words = s.split()
    return max(words, key=len) if words else ""



