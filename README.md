[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15426622&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

Python is an interpreted, object-orientated, high-level programming language with dynamic semantics.It is versatile as it is widely used for various purposes such as Data analysis, Web development, Artificial intellegence & machine learning, Education and many more.Python allows developers to focus on logic and algorithms without worrying about memory management, as it abstracts away low level details.It is free to use,modify and distribute and it runs on multiple operating systems.

   EXAMPLES:
   DATA ANALYSIS:Python has libraries like Pandas,Matplotlib etc. that make it an ideal choice for easy handling, analyzing, and visualizing of large datasets and making it easy to create interactive and dynamic visualizations.Python's extensive list of libraries facilitate AI and ML development. It has frameworks like Django, enabling rapid development of web applications.Python also has beginner friendly, easy to learn syntax making it the best option for automating tasks.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.


1.Open a web browser and navigate to the python.org (the official python website)
2.Navigate to Downloads and select windows operating system and download the latest version of Python
3.Locate the downloaded file and click run or double click it to run
4.On the installer window click on the box that says ' Add Python to PATH ' and install
5.Once installation has been completed, to verify, it open the command prompt window
6.Once the command prompt window is open, type in " python --version " and press Enter
  on screen the python version will be visible, to change directories use ' cd ' , to create a new directory use 'mkdir (projectname) ' and to create a virtul enbironment run ' python -m venv venv '

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

print("Hello, World!")

print() is a built-in Python function used to output text or information to the console, the parenthesis are used to enclose the arguments passed to the function.
"Hello, World!" is a string literal, which is the message that will be printed.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

1.Integers(int): Represents whole numbers like 15, 3, -6

age = 18
print(age)

2.Floats(float): Represents decimals eg.3.14535

my_float = 3.145
print(my_float)

3.Strings(str): blocks of text containing different characters

greeting = " hello! "
print(greeting)

4.Boolean(bool): statement with true or false answers

isLearningFun = true
print(isLearningFun)

5.Lists(list): an ordered collection of items

my_list = [1, 2, 3]
print(my_list)

6.Tuples(tuple)1: ordered, unmodifiable collection of items

my_tuple(1, 2, 3)
print(my_tuple)

7.Sets(set): unordered collection of items

my_set = {7, 8, 9}
print(my_set)

8.Dictionaries(dict): unordered collections of key-value pairs

my_dict = {"name" : "Mary", "age": 20}
print(my_dict)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

Conditional statements are used to execute various blocks of code based on certain conditions.The ' if ' statement is the most common, it executes block of code if the statement checks a condition and if it's true.
'if-else' statemebts executes code whether a condition is true or false.

Example:

x = 30
if x > 15
print("x is greater than 15")
else:
print("x is less than or equal to 15")

A 'for' loop iterates over a sequence and executes a block of code for each item.

example:

clothes = ["t-shirt", "dress", "pants", "skirt", "cardigan"]

for cloth in clothes
print(f"I love wearing my {cloth}")


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions in Python are reusable blocks of code that perform specific tasks, take arguments, and return values.They are useful for breaking down large programs into smaller manageable chunks, the same code can be used in different parts of a program without duplication. Functions can hide implementation details and only show a simple interface with the necessary information. They also help organize code making it more readable and understandable.

   def add_numbers(a, b):
     return a + b

   EXAMPLE:
   result = add_numbers(10,9)
   print(result) #Output: 19

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

LISTS: Are an ordered collection of items, it can contain duplicate items, and are denoted by square brackets []
DICTIONARIES: Are an unordered collection of key-value pairs, it cannot contain duplicate items, and are denoted by curly brackets {}

# Create a list of numbers
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9]

# Create a dictionary with some key-value pairs
person = {
   "name" : "Lulu"
   "age"  : "20"
   "city" : "Pretoria"
}

# Basic operations lists
print("Original list", numbers)

# append
numbers.append(10)
print("After append:", numbers)

# inserting an element
numbers.insert(0, 0)
print("After insert:", numbers)

# removing
numbers.remove(2)
print("After remove", numbers)

# index
print("Index of 3:", numbers.infex(3))

# occuramces
print("Count of 2:", numbers.count(2))

# Basic operations for dictionaries
print("Original dictionary:", person)

# key-value pair
person["country"] = "South Africa"

# add new key-value pair
print("Afterbadd:", person)

# value associated with the key 'name'
print("Name:", person["name"])

# value associated with the key 'age' using get ()
print("Age:", person.get("age"))

# update value associated with the key 'age'
person["age"] = 21
print("After update:", person)

# removing a key-value pair with the key
del person["city"]

# print the dictionary after removing
print("After remove:", person)

# print all keys
print("Keys:", person.keys())

# print all values
print("Values:", person.values())


 8  - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

Exception handling in Python is a mechanism to handle and manage runtime errors so that the regular flow of the application can be maintained.It allows developers to predict and handle errors gracefully, preventing any crashes or production of unexpected results.

def divide_numbers(a, b):
    try:
       result = a / b
   except ZeroDivisionError:
        print("Error: Division by zero is not allowed.")
         result = None
     finally:
      print("Execution of the try-except block is complete.") 
   return result

   num1 = 10 
   num2 = 0

print(f"Result of division:{divide_numbers(num1, num2)}")


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

A module is a single file that contains functions, classes, and variables.They can be imported and used in other scripts and are used to organize and reuse code.To use a module in a Python script, use the 'import' statement followed by the module name, which accesses it's functions, variables, and classes.A package is a directory that contains several modules.They are used to organize similar modules into a layered structure and can be imported and used in other scripts.

EXAMPLE:

import math

# using the sqrt function from the math module
number = 25

result = math.sqrt(25)
print(result)  #Output 5.0

# using the pi constant
print(math.pi)  #Output 3.141592


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

   Reading files:
   Use ' open() ' to open a file.To read the entire file content into a string using ' read() ' method.The 'readline' method is used to read a single line from the file.To read all lines from the file into a list use the ' readlines() ' method.

   Writing files:
   Use ' open() ' to open a file.To write a string to the file, use the ' write() ' method.Using the ' writelines() ' method you will be able to write a list of strings to the file.

   first script:
   # open file in read mode with open('example.txt', 'r' )
# read_file.py

   def read_file(filename) :
      try:
        with open(filename, 'r') as file:
              content = file.read()
              print(content)
         except FileNotFoundError:
           print(f"Error: File '{filename}' does not exist.")

# example usage
read_file("example.txt")


   second script:
   # write_file.py

   def write_file(filename, lines):
       try:
         with open(filename, 'w') as file:
             for line in lines:
              file.write(line + "\n")
       print(f"File '{filename}' written successfully.")
   except IOError:
      print(f"Error: Unable to write to file '{filename}' .")
          
   # Example usage
   lines = ["Hi!", "se-assignment-6"]
   write_file("example.txt, lines)


REFERENCES:
realpython.org
python.land
geeksforgeeks.org
w3schools.com
python.org



# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


