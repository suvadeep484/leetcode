# Variables 

## Variable declaration 

- To declare a varible we use the following syntax

  ```py
  message ="Hello, world!"
  print(message) ➡️ Hello, world!
  ```

## Naming convention

- In python we use camel casing , example 

  ```py
  my_variable_name = "suvadeep"
  ```

## Multiple Assignments 

- Python allows you to assign multiple variables in a single line. Just separate the variables with a comma, and the right-hand side values with a comma as well.

  ```python
  msg1, msg2 = "Hello", "World"
  ```

## Variable types 

- We can print the type of a variable or value using the `type()` function in Python

  ```python
  print(type(10)) ➡️ <class 'int'>
  ```

## Dynamic Typing 

- In Python a single variable's type can change throughout the code. This is called **dynamic typing**.

## Type Casting 

- A variable in Python can be converted to a different type using **type casting**

  ```python
  variable = 10.9
  print(int(variable))
  ```

- This code will output: `10`

- The variable `variable` is a floating-point number. The `int()` function converts it to an integer.

## Type Errors 

- We can't convert a string to an integer, unless the string is a number. This code will cause a **ValueError**.

  ```python
  message = "Hello"
  message = int(message)
  ```

## Empty Variable 

- If we want to declare a variable without a value, we can use the `None` keyword

  ```python
  var = None
  ```

