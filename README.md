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

Create a function that moves the first character of the string to the end while keeping all remaining characters in their original order.

The following functions and methods were used in this problem:

- `rotate_word(text)` - initial function
  
Sample: `rotate_word("python") `

- Using index slicing `text[start:stop]`, `text[1:]` was used, indicating to 'slice' the word python starting from the 2nd character (index 1) to the rest, resulting in "ython". Meanwhile, `text[0]` refers to the 1st character (index 0) of the word python, yielding "p."

- The two methods were then concatenated using the plus sign (`+`). So, the `return` function was defined as `text[1:] + text[0]`.

Sample result: `rotate_word("python") ` -> "ythonp"

**These functions and methods were combined to create a function that moves the first character of the string to the end, keeping all remaining characters in their original order, and were then printed.**

    def rotate_word(text):
        return text[1:] + text[0]
    print(rotate_word ("birthday"))


**B. USERNAME BUILDER PROBLEM**

Create a function named make_username(), accepting two strings: `first_name` and `last_name`. The function must: 
1. Convert all letters to lowercase;
2. Remove all spaces from the first name;
3. Remove all spaces from the last name; and
4. Join the processed first and last names using one period (.).

The following functions and methods were used in this problem:

- `make_username(first_name, last_name)` - initial function

Sample: `make_username("Ana Maria", "De Leon") `

- To convert the letters to lowercase, `.lower()` was used for both the `first_name` and `last_name` elements. So, `Ana Maria.lower()` yields to "ana maria", while `De Leon.lower()` yields to "de leon".

- Additionally, `.replace(old, new) ` was used to remove the spaces on the elements, by setting 'old' as `(" ")` referring to the space between the characters, and the 'new' to `("")` for no spaces anymore. Yielding `de leon.replace(" ", "") with "deleon".

- With those functions defined in the created variables `build_first` and `build_last`, these variables were then concatenated with a plus sign (`+`), with "." in between.
  
Sample result: `make_username("Ana Maria", "De Leon")` -> "anamaria.deleon"

**These functions and methods were used together to generate the appropriate usernames and were then printed.**

      def make_username (first_name, last_name):
    
        build_first = first_name.lower().replace(" ", "")
        build_last = last_name.lower().replace(" ", "")
    
            return build_first + "." + build_last
      print(make_username("Electronics", "Engineering"))
  

**C. BOOKEND SWAP PROBLEM**

 Return a new list in which the first and last elements have exchanged positions.

 The following functions and methods were used:  
 
  - `swap_bookends(items)` - initial function
    
 Sample list: `swap_bookends([1, 2, 3, 4, 5, 6]) `

  -  Using extended sequence unpacking, the list was unpacked into three variables:
     - `first` - the first element;
     - `middle` – a list containing the elements between the first and last ones; and
     - `last` – the last element.

The function was defined as `first, *middle, last = items ` - as the middle variable can include multiple elements, the character asterisk (`*`) is applied to group the elements together.

 - For the switching of last and first elements' positions, the `return` function was defined as `[last] + middle + [first]`.
 
Sample result: `swap_bookends([1, 2, 3, 4, 5, 6]) ` -> [6, 2, 3, 4, 5, 1]

**These functions and methods were used to assign the corresponding values from the author's given lists to their appropriate variables and were then printed.**

    def swap_bookends (items):
      first, *middle, last = items
    
        return [last] + middle + [first]
    print(swap_bookends ([4, 5, 6, 7, 8, 9]))


Thank you for reading!

To see the full python program for PA 1, click this link: https://github.com/letizhamiguel-cyber/ECE-2112-PA-1/blob/main/PA1.ipynb, download then run all cells. 

# README file History:

August 27, 2026 - .ipynb file uploaded to GitHub.

August 29, 2026 - Initial Formatting of README.

September 1, 2026 - Input of further README content.

September 2, 2026 - Finalization of README with file history and key details.
