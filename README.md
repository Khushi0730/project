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


# 9. Calculate simple interest<br>
def simple_interest(principal, rate, time):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return (principal * rate * time) / 100<br>

# 10. Check if string is palindrome<br>
def is_palindrome(s):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return s == s[::-1] <br>

<b><i>Medium Level Function Question</b></i><br>

# 1. Fibonacci series up to n terms<br>
def fibonacci(n):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a, b = 0, 1<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;series = []<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for _ in range(n):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;series.append(a)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a, b = b, a + b<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return series<br>

# 2. GCD of two numbers<br>
def gcd(a, b):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;while b:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a, b = b, a % b<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return a<br>

# 3. LCM of two numbers<br>
def lcm(a, b):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return abs(a * b) // gcd(a, b)<br>

# 4. Sum of digits of a number<br>
def sum_of_digits(n):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return sum(int(digit) for digit in str(abs(n)))<br>

# 5. Second largest element in list<br>
def second_largest(lst):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;unique = list(set(lst))<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;unique.sort()<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return unique[-2] if len(unique) >= 2 else None <br>

# 6. Frequency of characters in string<br>
def char_frequency(s):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;freq = {}<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for ch in s:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;freq[ch] = freq.get(ch, 0) + 1<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return freq<br>

# 7. Check if number is Armstrong<br>
def is_armstrong(n):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;digits = str(n)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;power = len(digits)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return n == sum(int(d) ** power for d in digits)<br>

# 8. Check if number is Perfect<br>
def is_perfect(n):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if n < 2:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return False<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;divisors = [i for i in range(1, n) if n % i == 0]<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return sum(divisors) == n<br>

# 9. Return sorted list without using sort()<br>
def manual_sort(lst):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for i in range(len(lst)):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for j in range(i + 1, len(lst)):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if lst[i] > lst[j]:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;lst[i], lst[j] = lst[j], lst[i]<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return lst<br>

# 10. Word with maximum length in string<br>
def max_length_word(s):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;words = s.split()<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return max(words, key=len) if words else ""<br>






