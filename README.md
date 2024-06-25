[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15326885&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

 >Python is a high-level, interpreted programming language known for its readability and simplicity. Its syntax is designed to be easy to understand and write, which makes it an excellent choice for beginners and experienced developers alike.

 Key features include:
 
>Readability and simplicity
>Interpreted language
>Dynamic typing
>Extensive standard library

Examples of use cases where Python is particularly effective:

>Web development: Using frameworks like Django and Flask.
>Data science and machine learning: Libraries such as NumPy, Pandas, and TensorFlow.
>Scripting and automation: Writing scripts to automate repetitive tasks.
>Software development: Building applications and tools.
>Scientific computing: Using libraries like SciPy and Matplotlib.


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

Steps to install Python on Windows:

>Download the installer from the official Python website: python.org.
>Run the installer and check the option "Add Python to PATH".
>Click "Install Now".
>After installation, open Command Prompt and type python --version to verify the installation.


Setting up a virtual environment:

>Open Command Prompt.
>Install virtualenv using pip install virtualenv.
>Create a virtual environment: python -m venv myenv.
>Activate the virtual environment:
    .On Windows: myenv\Scripts\activate.
    .On macOS/Linux: source myenv/bin/activate.
>To deactivate, simply run deactivate.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

     Python program:
     print("Hello, World!")

     Explanation:

      >print is a function that outputs text to the console.
      >"Hello, World!" is a string enclosed in double quotes.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

     Basic data types in Python:

       >int: Integer numbers (e.g., 5)
       >float: Floating-point numbers (e.g., 3.14)
       >str: Strings (e.g., "Hello")
       >bool: Boolean values (True or False)
       >list: Ordered, mutable collections (e.g., [1, 2, 3])
       >tuple: Ordered, immutable collections (e.g., (1, 2, 3))
       >dict: Key-value pairs (e.g., {"key": "value"})
       >set: Unordered collections of unique elements (e.g., {1, 2, 3})

Script demonstrating variables of different data types:

# Integer
a = 6
print(a, type(a))

# Float
b = 3.14
print(b, type(b))

# String
c = "Hello"
print(c, type(c))

# Boolean
d = True
print(d, type(d))

# List
e = [1, 2, 3]
print(e, type(e))

# Tuple
f = (4, 5, 6)
print(f, type(f))

# Dictionary
g = {"key": "value"}
print(g, type(g))

# Set
h = {7, 8, 9}
print(h, type(h))


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

     Example of an if-else statement:
     
     x = 20
    if x > 10:
       print("x is greater than 10")
    else:
       print("x is not greater than 10")

     Example of a for loop:

     numbers = [1, 2, 3, 4, 5]
   for number in numbers:
      print(number)



6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
  
     > Functions allow you to encapsulate code into reusable blocks. They make code more modular, readable, and easier to maintain.

     Function that takes two arguments and returns their sum:

          def add(a, b):
             return a + b

         # Example of calling the function
           result = add(3, 5)
           print(result)  

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

     Differences between lists and dictionaries:

      > Lists: Ordered collections of items, accessible by index.
      > Dictionaries: Unordered collections of key-value pairs, accessible by key.

     Script creating a list of numbers and a dictionary with key-value pairs:

              # List of numbers
             numbers = [1, 2, 3, 4, 5]
            print(numbers)

            # Dictionary with key-value pairs
               person = {
                 "name": "Nhlalala",
                 "age": 40,
                  "city": "Johannesburg"
                 }
              print(person)

           # Basic operations on the list
             numbers.append(6)
             print(numbers)

          # Basic operations on the dictionary
            person["age"] = 41
            print(person)


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

     > Exception handling allows you to handle errors gracefully without stopping the execution of the program.

     Example of using try, except, and finally blocks:

             try:
                result = 10 / 0
             except ZeroDivisionError:
                print("Cannot divide by zero")
            finally:
                print("This will always be executed")


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

      Concepts of modules and packages:

         > Module: A single Python file containing functions, classes, or variables.
         > Package: A collection of modules in a directory that includes a special __init__.py file.

     Example of importing and using a module math:

     import math

     # Using the sqrt function from the math module
     result = math.sqrt(16)
     print(result)  


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    Script that reads the content of a file and prints it to the console:

             with open('example.txt', 'r') as file:
                    content = file.read()
                     print(content)

    
Script that writes a list of strings to a file:

           lines = ["First line", "Second line", "Third line"]
           with open('output.txt', 'w') as file:
                for line in lines:
                file.write(line + "\n")
      

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


