---
title: Basic Data Types in Python
description: In this blog, we are going to look at basic data types of python language. 
date: 2023-04-04
image: cover.png
categories:
    - Python
tags:
    - Type-conversion
    - Variables
    - basic data-types

---

Hi everyone! Today we are looking at the basics of Python programming language. As we know every programming language has programming concepts like basic syntax, variables, data types, flow control etc.  

## Variables in Python

Now, we are talking about variables in Python. Before that, we need to understand what is the meaning of the variables. Simply, variables are a named place in the computer's main memory where a programmer can store data. And also, the programmer can retrieve stored data using the variable’s name. Also, the programmer can change content stored in a variable by a later statement. The programmers get to choose the variable name. But, in choosing a variable name we need to follow some rules in Python language.

1. The variable name must begin with a letter `A-Z`, `a-z` or an underscore sign `_`.
2. The variable name can have letters, numbers or underscore signs.
3. Variable names are case-sensitive
4. The keyword in Python `reserved word` can not be used.

These are the variable naming rules in the Python language. And also, when you are naming variables, you need to give a meaningful name to the variable name as possible. From that, we can improve the readability of our code. As a good programmer, you want to follow that.  Now, you know what is the meaning of the variables and what are the variable naming rules. Let’s look at how to define a variable in Python. You can define a variable like below,

```python
name = "Shehan"
age = 20
```

In the above code, you can see how to define a variable in Python. First, you can choose a name for the variable and put an equal sign in front of the variable name, then you can put the data you desired. You can store many types of data. At this moment, data types come to our playground.  

## Basic Data-Types in Python

As we know, every programming language has many data types. Python has numeric, string, sequence, binary, mapping, boolean and set data types. In this article, we are covering numeric, string and boolean data types only. In the next article, we can cover other data types. Numeric data types are used to store numeric data in Python. There are three parts to numeric data types such as integers, floats and complex numbers. If you need to store integer value you can store it as int data. And also, the float data type is used for storing decimal numbers and the complex data type can store complex numbers like `2j`. In the below, you can see numeric data types.

```python
x = 10 # int
y = 7.5 # float
z = 1j # complex
```

And also, we can do arithmetic operations between numeric variables.

```python 
x = 5
y = 10


a = x + y # Addition
b = x - y # Subtraction
c = x * y # Multiplication
d = x / y # Divition
```

In the string data type, we can store characters and texts in the variable. Remember, when you store string data, you need to put it within single or double quotes. If you did not it Python interpreter give an error. Also, we need concern few factors when using quotes.

1. When you open quotes, you must close them.
2. They need to balance. Which means if you open a single quote, you must close the quote using a single quote, not a double quote. 
3. And, you can not close quotes like this, 
    ```python
    text = "Python is 'awesome". It is very simple '
    ```

4. Sometimes, we want to use double quotes inside double quotes. Like this, 

    ```python
    text = "Python is "awesome". It is very simple "
    ```
    At this moment, we have two methods to do the above without error. First is using double quotes within single quotes like this,

    ```python
    text = 'Python is "awesome". It is very simple '
    ```

    The second method is can use the escape character `\`. You can use it before inner double quotes. Like below,

    ```python
    text = "Python is \"awesome\". It is very simple "
    ```

Alright! Our next data type is Boolean. It has two values only as True and False. The boolean data type is mostly used for conditional statements such as if statements. You can define boolean variables like this,

```python
x = True
y = False
```
Or

```python
x = 10 < 8
y = 5 >= 4
```

Here, we used comparison operators. In later articles, We talk about these comparison operators. 

## Type-conversion in Python

Now, let’s cover type conversion in Python language. Type conversion means you can convert a data type to another data type in Python. For that, we use a set of built-in functions in Python such as `int()`, `float()`, `complex()`,  `str()`, and `bool()`. Let’s look at a simple type conversion in Python code.

```python
text = "12"
number = int(text) # text variable converted to a number


age = 20
age_text = str(age) # age variable converted to a string


x = 1
x_exsists = bool(x) # x variable converted to a boolean


value = 10
decimal = float(value) # value variable converted to a float
complex_number = complex(value) # value variable converted to a complex
```

Try the above code on your IDE. Then, you can understand Python type conversion. Remember, in string-to-integer conversion, your string variable must consist only of numbers. For some reason,  If you try to convert characters to integers, python gives an error. Because that is impossible.

Well guys, today we cover a lot of stuff about Python variables, data types and type conversion. In the next article, I will cover various operators in the Python language. Goodbye 😉 .


