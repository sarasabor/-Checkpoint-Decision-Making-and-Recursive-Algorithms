# -Checkpoint-Decision-Making-and-Recursive-Algorithms


1. Leap Year Checker
This function checks if a given year is a leap year using if-else statements.

def is_leap_year(year):  
    if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):  
        return True  
    else:  
        return False  

# Example usage  
year = int(input("Enter a year: "))  
if is_leap_year(year):  
    print(f"{year} is a leap year.")  
else:  
    print(f"{year} is not a leap year.")  
2. Ticket Pricing
This program determines the price of a movie ticket based on the user's age using if-else statements.

def ticket_price(age):  
    if age <= 12:  
        return "$10"  
    elif age <= 17:  
        return "$15"  
    else:  
        return "$20"  

# Example usage  
age = int(input("Enter your age: "))  
price = ticket_price(age)  
print(f"The movie ticket price is: {price}")  
Recursion
1. Fibonacci Sequence
This recursive function generates the nth Fibonacci number.

def fibonacci(n):  
    if n <= 0:  
        return 0  
    elif n == 1:  
        return 1  
    else:  
        return fibonacci(n - 1) + fibonacci(n - 2)  

# Example usage  
n = int(input("Enter the position in Fibonacci sequence: "))  
print(f"The {n}th Fibonacci number is: {fibonacci(n)}")  
2. Palindrome Checker
This recursive function checks if a given string is a palindrome, ignoring spaces and capitalization.

def is_palindrome(s):  
    # Preprocess the string: remove spaces and convert to lowercase  
    s = ''.join(s.split()).lower()  
    
    # Base case  
    if len(s) <= 1:  
        return True  
    if s[0] != s[-1]:  
        return False  
    
    # Recursive case  
    return is_palindrome(s[1:-1])  

# Example usage  
input_string = input("Enter a string to check if it's a palindrome: ")  
if is_palindrome(input_string):  
    print(f'"{input_string}" is a palindrome.')  
else:  
    print(f'"{input_string}" is not a palindrome.')  
