---
title: Lecture 2
date: 2024-04-07
---

Download the <a href="/Introduction to Python/Lectures/Lecture_02/lecture2.pdf">PDF</a>

## Loops

Loops are used to repeat a block of code a certain number of times. 
- There are two types of loops in Python: `for` loops and `while` loops.
    - `for` loops are used to iterate over a sequence.
    - `while` loops are used to repeat a block of code while a condition is true.
- Loops are useful for automating repetitive tasks, iterating over data, and more.
- Loops can be broken out of using the `break` keyword.

### For Loops

`for` loops are used to iterate over a sequence.

The syntax for a `for` loop is as follows:

```Python
for <variable> in <sequence>:
    <code>
```

The `<variable>` is a variable that will be assigned to each element in the `<sequence>` one at a time. The `<code>` is the code that will be executed for each element in the `<sequence>`. The `<sequence>` can be a list, tuple, string, or any other iterable object.

Here is an example of a `for` loop:
        
```Python
for i in [1, 2, 3, 4, 5]:
    print(i)
```

This will print the numbers 1 through 5. The `<variable>` `i` is assigned to each element in the list one at a time. The `<code>` `print(i)` is executed for each element in the list.


Here is another example of a `for` loop:

```Python
for i in range(5):
    print(i)
```

This will print the numbers 0 through 4. The `range()` function returns a sequence of numbers. The `range()` function can take up to three arguments: `range(start, stop, step)`. The `start` argument is the number to start at (default is 0). The `stop` argument is the number to stop at (not included). The `step` argument is the number to increment by (default is 1).

Here is another example of a `for` loop:

```Python
for i in range(1, 10, 2):
    print(i)
```

This will print the odd numbers from 1 to 9. The `range()` function can be used to iterate over a sequence of numbers. The `range()` function can be used to iterate over a sequence of numbers.


### While Loops

`while` loops are used to repeat a block of code while a condition is true.

The syntax for a `while` loop is as follows:

```Python
while <condition>:
    <code>
```
The `<condition>` is a boolean expression that is evaluated each time the loop is run. The `<code>` is the code that will be executed while the `<condition>` is true.

 Here is an example of a `while` loop:

```Python
i = 0
while i < 5:
    print(i)
    i += 1


This will print the numbers 0 through 4. The `<condition>` `i < 5` is evaluated each time the loop is run. The `<code>` `print(i)` is executed while the `<condition>` is true. The `<code>` `i += 1` increments the variable `i` by 1 each time the loop is run.

### Nested Loops

Loops can be nested inside each other.

Here is an example of a nested `for` loop:

```Python
for i in range(5):
    for j in range(5):
        print(i, j)
```

This will print the numbers 0 through 4. The `<code>` `print(i, j)` is executed for each element in the list. The `<variable>` `i` is assigned to each element in the list one at a time. The `<variable>` `j` is assigned to each element in the list one at a time.

## Conditionals

Conditionals are used to execute a block of code if a condition is true. There are three types of conditionals in Python: `if` statements, `elif` statements, and `else` statements.
\item `if` statements are used to execute a block of code if a condition is true.
\item `elif` statements are used to execute a block of code if another condition is true.
\item `else` statements are used to execute a block of code if no other condition is true.

Conditionals are useful for executing code based on certain conditions. Conditionals can be nested inside each other.

### If Statements

`if` statements are used to execute a block of code if a condition is true. The syntax for an `if` statement is as follows:

```Python
if <condition>:
    <code>
```
The `<condition>` is a boolean expression that is evaluated. The `<code>` is the code that will be executed if the `<condition>` is true.

Here is an example of an `if` statement:

```Python
if x > 0:
    print("x is positive")
```
This will print `x is positive` if the variable `x` is greater than 0. The `<condition>` `x > 0` is evaluated. The `<code>` `print("x is positive")` is executed if the `<condition>` is true.

### Elif Statements

`elif` statements are used to execute a block of code if another condition is true. The syntax for an `elif` statement is as follows:

```Python
if <condition>:
    <code>
elif <condition>:
    <code>

The `<condition>` is a boolean expression that is evaluated. The `<code>` is the code that will be executed if the `<condition>` is true.

Here is an example of an `elif` statement:

```Python
if x > 0:
    print("x is positive")
elif x < 0:
    print("x is negative") 
```

This will print `x is positive` if the variable `x` is greater than 0. This will print `x is negative` if the variable `x` is less than 0. The `<condition>` `x > 0` is evaluated. The `<code>` `print("x is positive")` is executed if the `<condition>` is true. The `<condition>` `x < 0` is evaluated. The `<code>` `print("x is negative")` is executed if the `<condition>` is true.

### Else Statements

`else` statements are used to execute a block of code if no other condition is true. The syntax for an `else` statement is as follows:

```Python
if <condition>:
    <code>
elif <condition>:
    <code>
else:
    <code>
```

The `<condition>` is a boolean expression that is evaluated. The `<code>` is the code that will be executed if the `<condition>` is true.

Here is an example of an `else` statement:

```Python
if x > 0:
    print("x is positive")
elif x < 0:
    print("x is negative")
else:
    print("x is zero")
```

### Nested Conditionals

Conditionals can be nested inside each other. This means that conditionals can be inside other conditionals. Here is an example of nested conditionals:

```Python
if x > 0:
    if x > 10:
        print("x is greater than 10")
    else:
        print("x is between 0 and 10")
else:
    print("x is less than or equal to 0")
```

Here is another example of nested conditionals:

```Python
if x > 0:
    if x > 10:
        print("x is greater than 10")
    elif x > 5:
        print("x is between 5 and 10")
    else:
        print("x is between 0 and 5")
else:
    print("x is less than or equal to 0")
```