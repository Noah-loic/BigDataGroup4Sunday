# 🧠 Introduction to Big Data Analytics — Quiz 1 Solutions
  
**Instructor**: Eric Maniraguha   
**Group**: 4  
 

This repository contains well-documented Python solutions to selected questions from **Quiz 1** in the course *Introduction to Big Data Analytics*. Below are solutions to:

- ✅ Question II: Palindrome Checker
- ✅ Question III: Iterating Over Two Text Inputs

---

## ✅ Question II: Check Palindrome

### ✍️ Problem Statement

Write a Python function that:

1. Asks the user to input a **string**.
2. Checks if the string is a **palindrome** (reads the same forwards and backwards).
3. Prints the result:  
   - `"Yes, it is a palindrome"`  
   - `"No, it is not a palindrome"`

### 🧾 Solution Code

```python
<pre> ```
def check_palindrome():
    text = input("Enter a string: ")
    normalized = text.replace(" ", "").lower()
    if normalized == normalized[::-1]:
        print("Yes, it is a palindrome.")
    else:
        print("No, it is not a palindrome.")

check_palindrome()
    ``` </pre>
