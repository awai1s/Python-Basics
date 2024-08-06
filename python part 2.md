# Python for ML and AI
## Part 2

### Contents
- [Python for ML and AI](#python-for-ml-and-ai)
  - [Part 2](#part-2)
    - [Contents](#contents)
  - [Variables and Data Types](#variables-and-data-types)
    - [Data Types](#data-types)
  - [Basic Operators](#basic-operators)

## Variables and Data Types

Variables in Python are used to store data values. A variable is essentially a name given to a memory location. Here’s how to declare and use variables:

1. **Declaring Variables:**
   ```python
   variable_name = value
   ```

2. **Dynamic Typing:** Python is dynamically typed, meaning you don’t need to declare the type of a variable. The interpreter automatically understands the data type based on the assigned value.

### Data Types
Data Types are classifications of data items. Python has several built-in data types:

1. **Numeric Types:**
   - **int:** Integer numbers
     ```python
     age = 19
     ```
   - **float:** Floating-point numbers
     ```python
     pi = 3.14
     ```

2. **Text Type:**
   - **str:** String, a sequence of characters
     ```python
     name = "Awais"
     ```

3. **Boolean Type:**
   - **bool:** Boolean values (True or False)
     ```python
     is_student = True
     ```

4. **Sequence Types:**
   - **list:** Ordered collection of items
     ```python
     fruits = ["apple", "banana", "cherry"]
     ```
   - **tuple:** Ordered, immutable collection of items
     ```python
     coordinates = (10, 20)
     ```
   - **range:** Sequence of numbers
     ```python
     numbers = range(5)
     ```

5. **Mapping Type:**
   - **dict:** Unordered collection of key-value pairs
     ```python
     person = {"name": "Awais", "age": 19}
     ```

6. **Set Types:**
   - **set:** Unordered collection of unique items
     ```python
     unique_numbers = {1, 2, 3}
     ```
   - **frozenset:** Immutable version of a set
     ```python
     frozen_numbers = frozenset([1, 2, 3])
     ```

## Basic Operators
Operators are special symbols that perform operations on variables and values. Python includes several types of operators:

1. **Arithmetic Operators:** These operators perform basic arithmetic operations.
   - **Addition (`+`):** Adds two operands
     ```python
     sum = 10 + 5  # Result: 15
     ```
   - **Subtraction (`-`):** Subtracts the second operand from the first
     ```python
     difference = 10 - 5  # Result: 5
     ```
   - **Multiplication (`*`):** Multiplies two operands
     ```python
     product = 10 * 5  # Result: 50
     ```
   - **Division (`/`):** Divides the first operand by the second
     ```python
     quotient = 10 / 5  # Result: 2.0
     ```
   - **Exponent (`**`):** Raises the first operand to the power of the second
     ```python
     power = 10 ** 2  # Result: 100
     ```
   - **Remainder (`%`):** Returns the remainder of the division
     ```python
     remainder = 10 % 3  # Result: 1
     ```

2. **Comparison Operators:** These operators compare two values and return a Boolean result (True or False).
   - **Equal to (`==`):** Checks if two operands are equal
     ```python
     is_equal = (10 == 5)  # Result: False
     ```
   - **Not equal to (`!=`):** Checks if two operands are not equal
     ```python
     is_not_equal = (10 != 5)  # Result: True
     ```
   - **Greater than (`>`):** Checks if the first operand is greater than the second
     ```python
     is_greater = (10 > 5)  # Result: True
     ```
   - **Less than (`<`):** Checks if the first operand is less than the second
     ```python
     is_less = (10 < 5)  # Result: False
     ```
   - **Greater than or equal to (`>=`):** Checks if the first operand is greater than or equal to the second
     ```python
     is_greater_or_equal = (10 >= 5)  # Result: True
     ```
   - **Less than or equal to (`<=`):** Checks if the first operand is less than or equal to the second
     ```python
     is_less_or_equal = (10 <= 5)  # Result: False
     ```

3. **Logical Operators:** These operators combine conditional statements.
   - **and:** Returns True if both statements are true
     ```python
     result = (10 > 5) and (10 < 15)  # Result: True
     ```
   - **or:** Returns True if one of the statements is true
     ```python
     result = (10 > 5) or (10 > 15)  # Result: True
     ```
   - **not:** Reverses the result, returns False if the result is true
     ```python
     result = not(10 > 5)  # Result: False
     ```