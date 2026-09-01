# Introduction to Python
## Description
This lesson is about learning the basic code and functions in Python. It also shows how to use them to make simple programs.

## Intended Learning Outcomes
At the end of this laboratory activity, the student should be able to:
1. use basic Python functions, operators, and string operations;
2. manipulate strings using indexing, slicing, and built-in string methods;
3. apply sequence unpacking to manipulate the elements of a list; and
4. construct simple Python functions that return a specified result.

---------------------
## 1. Word Rotation Problem
In this problem, the goal is to create a function that accepts a word from the user. The output should contain the user input, but the first character is moved to the end while the remaining characters stay the same.

### Code
```python
def rotate_word(word):
    print(input_data[1:] + input_data[0])

input_data = input('Give word: ')

rotate_word(input_data)
```
The program uses the function rotate_word. Outside the function, the program asks users for an input word of their choice. The function is then called to process the data it is given. Finally, it prints the rotated word.

-------------------------------
## 2. Username Builder Problem
In this problem, the goal is to make a username based on what the user inputs. It will undergo the process of converting all letters to lowercase and removing all the spaces from the first and last name.

### Code
```python
def make_username(first_name, last_name):
    lower_first = first.lower()
    lower_last = last.lower()
    full_name = ".".join([lower_first, lower_last])
    print(full_name.replace(" ", ""))

first = input("Input your first name: ")
last = input("Input your last name: ")

make_username(first, last)
```
The program uses the make_username function with a parameter of first_name and last_name inside the parenthesis. Outside the function, the program will ask the user for their first and last name separately. After storing the data in their respective variable, it will call the function. The function will then undergo the process of converting all the letters to lowercase and joining them in the processed first and last names using one period (.). Finally, it will print the username, removing the spaces in between.

--------------------------
## 3. Bookend Swap Problem
In this problem, the goal is to ask for a user input of at least two elements. This input will then unpack into three variables: the first, middle, and the last. The output should show that the first and last elements are swapped while the middle stays in order.

### Code
```python
def swap_bookends(items):
    first = List[-1]
    middle = List[1:-1]
    last = List[0]
    print(first, *middle, last)

user_input = input("Write down your list: ")
List = user_input.split()

swap_bookends(List)
```
The program uses the swap_bookends function, which accepts a parameter named items. Outside the function, user input is stored in a variable and converted into a list before being passed to the function. Inside, the list is unpacked into three variables: first (containing the last element), last (containing the first element), and middle (containing the remaining elements). Finally, the function prints the updated list.
