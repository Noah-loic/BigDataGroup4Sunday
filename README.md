#  Group Assignment: String Handling in Python

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

##  Problem 2 – Palindrome Checker

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
## Example Usage

```python
# Example 1: Palindrome input
Enter a string: Racecar
Yes, it is a palindrome.

# Example 2: Non-palindrome input
Enter a string: Hello
No, it is not a palindrome.

# Example 3: Phrase with spaces
Enter a string: A man a plan a canal Panama
Yes, it is a palindrome.
```
##  Problem 3 – Combine and Process Two Texts

###  Problem Statement

1. Ask the user to enter **two separate texts**
2. Combine the two texts into one
3. Iterate over each character in the combined text
4. Return the characters as a `list`
5. Display:

> Thank you for using my application.  
> After processing the input.

###  Code

```python
def merged_process():
    text1 = input("Enter first text: ")
    text2 = input("Enter second text: ")
    combined_text = text1 + text2
    characters = list(combined_text)
    
    print("Characters in the combined text:")
    print(characters)
    
    print("Thank you for using my application.")
    print("After processing the input.")
    
    return characters

# Call the function
merged_process()
```
## Code Explanation

The script consists of a single function, `merged_process()`, which performs the following steps:

1. **User Input**:
   - The function uses `input("Enter first text: ")` and `input("Enter second text: ")` to prompt the user for two strings.
   - The first input is stored in the variable `text1`, and the second in `text2`.

2. **String Combination**:
   - The inputs are combined using `text1 + text2`, which joins the two strings end to end.
   - The result is stored in the variable `combined_text`.
   - For example, if the user enters `"Hello"` and `"World"`, the combined result will be `"HelloWorld"`.

3. **Character Iteration**:
   - The combined string is passed to the `list()` function using `characters = list(combined_text)`.
   - This creates a list where each element is a single character from the combined text.
   - Example:
     - Combined text: `"HelloWorld"`
     - Characters list: `['H', 'e', 'l', 'l', 'o', 'W', 'o', 'r', 'l', 'd']`

4. **Output**:
   - The function prints:
     - `"Characters in the combined text:"` — a label for clarity.
     - The list of characters — which shows the result of the iteration.
     - `"Thank you for using my application."` — a user-friendly message.
     - `"After processing the input."` — a closing message to indicate the end of the operation.

5. **Return Value**:
   - The function uses `return characters` to return the list of characters. This makes the function reusable in other parts of a program, though it’s not required by the user.

6. **Function Execution**:
   - The function is executed with `merged_process()` immediately after its definition, allowing the user to interact with the program.

## Example Usage

```python
# Example input:
Enter first text: Hello
Enter second text: World

# Output:
Characters in the combined text:
['H', 'e', 'l', 'l', 'o', 'W', 'o', 'r', 'l', 'd']
Thank you for using my application.
After processing the input.
```

##  Final Notes

We successfully implemented the required functions using clean and efficient Python syntax.  


