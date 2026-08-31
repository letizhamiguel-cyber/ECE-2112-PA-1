# ECE-2112-PA-1
**Made by: MIGUEL, Letizha Martha C. | Section: 2ECE-D**

The content of this repository contains the Experiment 1: Introduction to Python Programming for the course ECE 2112: Advanced Programming, this S.Y. 2026-2027. This project covers three python problems pertaining to Module 1 - Introduction to Python. 

# Intended Learning Outcomes

At the end of this laboratory activity, the student should be able to:
1. Use basic Python functions, operators, and string operations;
2. Manipulate strings using indexing, slicing, and built-in string methods;
3. Apply sequence unpacking to manipulate the elements of a list; and
4. Construct simple Python functions that return a specified result.

# Programming Problems

**A. WORD ROTATION PROBLEM**

Create a function that moves the first character of the string to the end while keeping all remaining characters in their original order. The function shall be named rotate_word(), and the capitalization of every character shall be preserved.

The following functions and methods were used in this problem:

- `rotate_word(text)` -

  Example: `rotate_word("python") ` -> "ythonp"

This built-in function and method were combined in order to create a single defined function that sorts the letters of a word alphabetically;

    \\code


**B. USERNAME BUILDER PROBLEM**

Create a function named make_username(), accepting two strings: `first_name` and `last_name`
function must: 
1. Convert all letters to lowercase;
2. Remove all spaces from the first name;
3. Remove all spaces from the last name; and
4. Join the processed first and last names using one period (.).

The following functions and methods were used in this problem:

- `make_username(first_name, last_name)` -

  Example: `make_username("Ada", "Lovelace") ` -> "ada.lovelace"

       \\code
  

**C. BOOKEND SWAP PROBLEM**

 Return a new list in which the first and last elements have exchanged positions.

 The following functions and methods were used:  
 
  - `swap_bookends(items)` - the named function
    
 Sample list: `swap_bookends([1, 2, 3, 4, 5, 6]) `

  -  Using extended sequence unpacking, the list was unpacked into three variables:
     - `first` - the first element;
     - `middle` – a list containing everything between the first and last elements; and
     - `last` – the last element.

The function was defined as `first, *middle, last = items ` - as the middle variable can include multiple elements, the character asterisk (*) is applied to group the elements together.

 - For the switching of last and first elements' positions, the `return` function was defined as `[last] + middle + [first]`
 
 Example: `swap_bookends([1, 2, 3, 4, 5, 6]) ` -> [6, 2, 3, 4, 5, 1]

**These functions and methods were used to assign the corresponding values from the author's given lists to their appropriate variables and print them.**

    def swap_bookends (items):
    first, *middle, last = items
    
        return [last] + middle + [first]
    print(swap_bookends ([4, 5, 6, 7, 8, 9]))


 
