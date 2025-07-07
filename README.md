# 📘 Group Assignment: String Handling in Python

## Course Information

**Course**: _Intro to Big Data Analytics_  
**Assignment**: **String Handling (Problem 2 & 3)**  
**Group Name**: _[Group 4]_  
**Date**: _[6th/07/2025]_

## Group Members

1. **[IRADUKUNDA Immaculee: 27378]**
2. **[KIZUNGU SHYAKA Noah Loic: 25919]**
3. **[RUKESHA Prince: 26474]**
4. **[ISHIMWE Prince Cuthbert: 27089]**
5. **[MURENZI Charles: 26680]**
36. **[Nadjilem Nayam Oscar: 26518]**

---

## Assignment Summary

> This assignment required implementing string operations in Python using functions, user input, and collections.  
>
>> We solved:
>> 
>> 1. **Palindrome Checker**  
>> 2. **Text Combination & Character Iteration**

---

## 📌 Problem 2 – Palindrome Checker

### Problem Statement

* Write a function that asks the user to enter a string.  
* If the string is a **palindrome** (reads the same forward and backward), print:  
  > _Yes, it is a palindrome._  
* Otherwise, print:  
  > _No, it is not a palindrome._

### Code

```python
def check_palindrome():
    text = input("Enter a string: ")
    normalized = text.replace(" ", "").lower()
    if normalized == normalized[::-1]:
        print("Yes, it is a palindrome.")
    else:
        print("No, it is not a palindrome.")

check_palindrome()
```
## Code Explanation

The script consists of a single function, `check_palindrome()`, which performs the following steps:

1. **User Input**:
   - The function uses `input("Enter a string: ")` to ask the user to enter a string.
   - The entered string is stored in the variable `text`.

2. **String Normalization**:
   - The input string is processed using `text.replace(" ", "").lower()`:
     - `replace(" ", "")` removes all spaces from the string to ensure phrases like "A man a plan" are treated as a single continuous string ("Amanaplan").
     - `lower()` converts the string to lowercase to make the comparison case-insensitive (e.g., "Racecar" becomes "racecar").
   - The normalized string is stored in the variable `normalized`.

3. **Palidrome CHeck**
  - The function checkks if the normalized string is equal to its reverse using `normalized == normalized[::-1]`:
    - The slice `[::1]` creates a reversed copy of the string by going through it backward.
    - If the normalized string equals its reverse, it is palindrome.
- For ecample, for the input "Racecar"
 - Normalized: "racecar"
 - Reverse: "racecar"
 - Since they match, it is a palindrome.

4. **Output**:
   - If the condition `normalized == normalized[::-1]` is `True`, the function prints: `"Yes, it is a palindrome."`
   - Otherwise, it prints: `"No, it is not a palindrome."

5. **Function Execution**:
   - The function is called immediately after its definition with `check_palindrome()`, prompting the user to enter a string and running the palindrome check.
