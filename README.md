# BigDataGroup4Sunday
Assignment Summary
This assignment required implementing string operations in Python using functions, user input, and collections.

We solved:

Palindrome Checker

Text Combination & Character Iteration

– Palindrome Checker
Problem Statement
Write a function that asks the user to enter a string.

If the string is a palindrome (reads the same forward and backward), print:

Yes, it is a palindrome.

Otherwise, print:

No, it is not a palindrome.

Codes:
def check_palindrome():
    text = input("Enter a string: ")
    normalized = text.replace(" ", "").lower()
    if normalized == normalized[::-1]:
        print("Yes, it is a palindrome.")
    else:
        print("No, it is not a palindrome.")

check_palindrome()
