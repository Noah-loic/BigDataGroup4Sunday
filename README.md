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
