# Python for ML and AI
## Part 3

Written by:

**Syed Muhammad Awais Raza**
 [LinkedIn](https://www.linkedin.com/in/syed-muhammad-awais-raza-905317278/) | 
   [Email](mailto:awaisraza5424@gmail.com) | [GitHub](https://github.com/awai1s)
### Contents
1. [Conditional Statements (if, elif, else)](#conditional-statements-if-elif-else)
2. [Loops (for, while)](#loops-for-while)

## Conditional Statements (if, elif, else)
Conditional statements allow you to execute specific blocks of code based on certain conditions. Python provides three main types of conditional statements: `if`, `elif`, and `else`.

### 1. The if Statement
The `if` statement evaluates a condition and executes the block of code inside it if the condition is True.

```python
age = 20
if age >= 18:
    print("You are an adult.")
```

### 2. The elif Statement
The `elif` (short for else if) statement allows you to check multiple conditions.

```python
score = 85
if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
else:
    print("Grade: D")
```

### 3. The else Statement
The `else` statement catches anything which isn't caught by the preceding conditions.

```python
temperature = 25
if temperature > 30:
    print("It's hot.")
else:
    print("It's not hot.")
```

### Examples of Conditional Statements

**Example 1: Checking if a number is positive, negative, or zero**

```python
number = 0
if number > 0:
    print("Positive")
elif number < 0:
    print("Negative")
else:
    print("Zero")
```

**Example 2: Checking if a person is eligible to vote**

```python
age = 17
if age >= 18:
    print("Eligible to vote")
else:
    print("Not eligible to vote")
```

## Loops (for, while)
Loops are used to repeat a block of code multiple times. Python provides two types of loops: `for` and `while`.

### 1. The for Loop
The `for` loop iterates over a sequence (like a list, tuple, or string) and executes the block of code for each item in the sequence.

**Example 1: Iterating over a list**

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

**Example 2: Iterating over a range of numbers**

```python
for i in range(5):
    print(i)
```

### 2. The while Loop
The `while` loop continues to execute the block of code as long as the condition is True.

**Example 1: Printing numbers from 1 to 5**

```python
i = 1
while i <= 5:
    print(i)
    i += 1
```

**Example 2: Breaking out of a loop when a condition is met**

```python
i = 1
while i <= 10:
    print(i)
    if i == 5:
        break
    i += 1
```

### Using break and continue
- **The break statement** terminates the loop.
- **The continue statement** skips the current iteration and proceeds to the next one.

**Using break**

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

**Using continue**

```python
for i in range(10):
    if i % 2 == 0:
        continue
    print(i)
```

### Examples of Loops

**Example 1: Sum of the first 10 natural numbers**

```python
sum = 0
for i in range(1, 11):
    sum += i
print(f"Sum of the first 10 natural numbers: {sum}")
```

**Example 2: Finding the factorial of a number using a while loop**

```python
number = 5
factorial = 1
i = 1
while i <= number:
    factorial *= i
    i += 1
print(f"Factorial of {number} is {factorial}")
```