# Python for ML and AI
## Part 4

Written by:

**Syed Muhammad Awais Raza**
 [LinkedIn](https://www.linkedin.com/in/syed-muhammad-awais-raza-905317278/) | 
   [Email](mailto:awaisraza5424@gmail.com) | [GitHub](https://github.com/awai1s)
   
### Contents
- [Python for ML and AI](#python-for-ml-and-ai)
  - [Part 4](#part-4)
    - [Contents](#contents)
  - [Defining and Calling Functions](#defining-and-calling-functions)
    - [Defining a Function](#defining-a-function)
    - [Example](#example)
  - [Importing and Using Modules](#importing-and-using-modules)
    - [Importing a Module](#importing-a-module)
    - [Example](#example-1)
    - [Creating and Importing Your Own Module](#creating-and-importing-your-own-module)
  - [Lists and Tuples](#lists-and-tuples)
    - [Lists](#lists)
    - [Tuples](#tuples)
  - [Dictionaries and Sets](#dictionaries-and-sets)
    - [Dictionaries](#dictionaries)
    - [Sets](#sets)
  - [String Operations and Methods](#string-operations-and-methods)
    - [Basic String Operations](#basic-string-operations)
    - [Common String Methods](#common-string-methods)
    - [Formatting Strings](#formatting-strings)

## Defining and Calling Functions
Functions are reusable blocks of code that perform a specific task. They help in organizing code, making it more readable and maintainable.

### Defining a Function
To define a function, use the `def` keyword followed by the function name and parentheses. Inside the parentheses, you can define parameters that the function can accept.

```python
def greet(name):
    """
    Function to greet a person with their name.
    """
    print(f"Hello, {name}!")

# Calling the function
greet("Awais")
```

### Example

```python
def add(a, b):
    """
    Function to add two numbers and return the result.
    """
    return a + b

result = add(3, 5)
print(f"The sum is: {result}")
```

## Importing and Using Modules
Modules are files containing Python code that can be imported and used in other Python scripts. Python comes with a vast standard library of modules, and you can also create your own.

### Importing a Module
Use the `import` keyword to import a module.

```python
import math

# Using a function from the math module
print(f"The value of pi is: {math.pi}")
```

### Example

```python
import random

# Generating a random number between 1 and 10
random_number = random.randint(1, 10)
print(f"Random number: {random_number}")
```

### Creating and Importing Your Own Module
Create a file named `my_module.py` with the following content:

```python
# my_module.py

def say_hello():
    return "Hello from my_module!"
```

In another Python script, import and use your module:

```python
import my_module

print(my_module.say_hello())
```

## Lists and Tuples
Data structures are used to store and organize data efficiently.

### Lists
Lists are mutable, ordered collections of items. They can contain elements of different data types.

```python
# Creating a list
fruits = ["apple", "banana", "cherry"]

# Accessing elements
print(fruits[0])  # Output: apple

# Modifying elements
fruits[1] = "blueberry"
print(fruits)  # Output: ['apple', 'blueberry', 'cherry']

# Adding elements
fruits.append("orange")
print(fruits)  # Output: ['apple', 'blueberry', 'cherry', 'orange']
```

### Tuples
Tuples are immutable, ordered collections of items. They are similar to lists but cannot be modified after creation.

```python
# Creating a tuple
colors = ("red", "green", "blue")

# Accessing elements
print(colors[1])  # Output: green

# Tuples cannot be modified
# colors[1] = "yellow"  # This will raise an error
```

## Dictionaries and Sets

### Dictionaries
Dictionaries are mutable, unordered collections of key-value pairs. Keys must be unique and immutable.

```python
# Creating a dictionary
student = {"name": "Awais", "age": 21, "major": "AI"}

# Accessing elements
print(student["name"])  # Output: Awais

# Modifying elements
student["age"] = 22
print(student)  # Output: {'name': 'Awais', 'age': 22, 'major': 'AI'}

# Adding elements
student["grade"] = "A"
print(student)  # Output: {'name': 'Awais', 'age': 22, 'major': 'AI', 'grade': 'A'}
```

### Sets
Sets are mutable, unordered collections of unique items. They are useful for membership testing and eliminating duplicate entries.

```python
# Creating a set
numbers = {1, 2, 3, 4, 5}

# Adding elements
numbers.add(6)
print(numbers)  # Output: {1, 2, 3, 4, 5, 6}

# Removing elements
numbers.remove(2)
print(numbers)  # Output: {1, 3, 4, 5, 6}
```

## String Operations and Methods
Strings are sequences of characters. Python provides many operations and methods to work with strings.

### Basic String Operations

```python
# Creating a string
text = "Hello, World!"

# Accessing characters
print(text[0])  # Output: H

# Slicing strings
print(text[0:5])  # Output: Hello

# Concatenating strings
greeting = "Hello"
name = "Awais"
message = greeting + ", " + name + "!"
print(message)  # Output: Hello, Awais!
```

### Common String Methods

```python
# Converting to uppercase
print(text.upper())  # Output: HELLO, WORLD!

# Converting to lowercase
print(text.lower())  # Output: hello, world!

# Replacing substrings
print(text.replace("World", "Python"))  # Output: Hello, Python!

# Splitting strings
words = text.split(", ")
print(words)  # Output: ['Hello', 'World!']
```

### Formatting Strings
Python provides several ways to format strings, making it easier to create formatted text.

**Using the `format()` Method**

```python
name = "Awais"
age = 19
message = "My name is {} and I am {} years old.".format(name, age)
print(message)  # Output: My name is Awais and I am 19 years old.
```

**Using f-Strings (Python 3.6+)**

```python
name = "Awais"
age = 19
message = f"My name is {name} and I am {age} years old."
print(message)  # Output: My name is Awais and I am 19 years old.
```