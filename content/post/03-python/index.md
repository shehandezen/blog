---
title: Operators in Python
description: In this blog, we are going to cover operators in Python language. 
date: 2023-04-05
image: cover.png
categories:
    - Python
tags:
    - Operators
    - String Slicing
    - String Concatenation

---

Ok, In this article, we will cover operators in Python language as I mentioned in the previous article. As we know, every programming language has a bunch of operators. Python also has a lot of operators to perform different operations. First, let’s understand what are operators, and how many types of operators Python has. Basically, operators are special symbols that are designated to perform some sort of computation. The values that operators act on are called operands. For demonstrating this, look at the below Python code,

```python
x = 7 + 8
y = 6 + 9 * 4 (8/2)
```

Above, `+`, `*`, and `/` are the operators and other all digits are operands.  Because operators act on that digits. Now, you may have some idea about operators. Python has many types of operators such as arithmetic, assignment, comparison, logical, identity, membership, and bitwise operators. Let’s look at each type of operators.

## Arithmetic Operators

As we well know, arithmetic operators are used for computing common mathematical operations like addition, subtraction, multiplication, division, exponentiation, etc. Below you can find many arithmetic operators,

| Operator | Description    |
|----------|----------------|
|   +      |  Addition      |
|   -      | Subtraction    |
|   *      | Multiplication |
|   /      | Division       |
|   %      | Modulus        |
|   **     | Exponentiation |
|   //     | Floor Division |
 

let’s try these on Python. 

```python
x = 5
y = 10


a = x + y # Addition
b = x - y # Subtraction
c = x * y # Multiplication
d = x / y # Division
e = x % y # Modulus
f = x ** y # Exponentiation
g = x // y # Floor Division
```

Here, addition, subtraction, multiplication and division are the basic arithmetic operators. But, modulus, exponentiation and floor division are just different. The modulus operator is used to get the remainder of a division and exponentiation returns the result of the first operand to the power second operand.  The floor division is mostly the same as the common division. But floor division is quite different to the common division. 
The floor division returns the smallest integer less than or equal to the result of the common division. Let’s move to the next type of operators called comparison operators
 
## Comparison Operators

Briefly, the comparison operators are used to compare two values. Always, comparison operations return a boolean value. Example code in the below,

```python
a = 7 == 5 # equal to
b = 7 != 5 # not equal
c = 7 > 5 # greater than
d = 7 >= 5 # greater than or equal to
e = 7 < 5 # less than or equal to
f = 7 <= 5 # less than
```

These are the comparison operators.

| Operator | Description               |
|----------|---------------------------|
|   >      |  Greater than             |
|   <      | Less than                 |
|   ==     | Equal to                  |
|   !=     | Not equal to              |
|   >=     | Greater than or equal to  |
|   <=     | Less than or equal to     |
 

## Logical Operators

The logical operators can combine conditional statements and boolean values. And also, return a boolean value.

| Operators  | Description   | Syntax   |    
|------------|---------------|----------|
| and        | Logical AND   | X and Y  |   
| or         | Logical OR    | X or Y   |   
| not        | Logical NOT   | X not Y  | 

## Bitwise Operators

When you deal with binary numbers, bitwise operators are very useful for doing binary operations.  The bitwise operators perform bit-by-bit operations on the binary numbers.

|Operator    |      Description                                                                                         | Syntax    |
|------------|----------------------------------------------------------------------------------------------------------|-----------|
| &          | Bitwise AND                                                                                              | X & Y     |
| &#124;     | Bitwise OR                                                                                               | X &#124; Y|
| ~          | Bitwise NOT                                                                                              | X ~ Y     |
| ^          | Bitwise XOR                                                                                              | X ^ Y     |
| >>         | Shift left by pushing zeros in from the right and let the leftmost bits fall off                         | X >> Y    |
| <<         | Shift right by pushing copies of the leftmost bit in from the left, and let the rightmost bits fall off  | X << Y    |

## Identity Operators

The identity operator checks if two objects are the same or located in the same main memory location. Those also return a boolean value. The identity operator symbolizing by the `is` keyword. You can check two variables in the same location like below,

```python
x = 10
y = 25


z = x is y # True if the variables are the same
z = x is not y # True if the variables are not the same
```

## Membership Operators

When using data collection, sometimes we want to check a specific value or a variable that exists in the data collection. At that moment, we can use the membership operator to do that. `in` keyword represents the membership operator. If you want to check the value or variable does not exist in the data collection. You can put the `not` keyword before the `in` keyword. Remember, when using the identity operator first you need to put the data collection and then you can put the `in` or `not in`  keywords as you want. After, put the variable or value. You can see it in the below example code,

```python
x = [1,5,3,7,6,9,4]
y = 7


z = y in x # True if exist
z = y not in x # True if does not exist
```

## Assignment Operators

Already, we had used an assignment operator `=`. Assignment operators are used to assigning a value to the variable. Simply, you can do it using the `=` sign. The equal sign is the basic assignment operator in Python. But, just think you need to do whatever operation while assigning it to a variable, it can be an arithmetic operation, a logical operation, a bitwise operation, or a comparison operation. You can easily understand by the below example,

```python
n = n + 1
```

In some iterations, we use like above statements. In that statement, one adds to the `n`  variable and its result assign to that `n` variable. We can easily do it using other assignment operators.  Those are in the below,

| Operator  | Alternative    |
|-----------|----------------|
| +=        | a = a + b      |
| -=        | a = a - b      |
| *=        | a = a * b      |
| /=        | a = a / b      |
| %=        | a = a % b      |
| //=       | a = a // b     |
| **=       | a = a ** b     |
| &=        | a = a & b      | 
| &#124;=   | a = a &#124; b |
| ^=        | a = a ^ b      |
| >>=       | a = a >> b     |
| <<=       | a = a << b     |

## Operator Precedence

The operator precedence is the order in which operations are performed. That is so important because, if you do not follow that precedence you can not get your expected result. In the below table, you can get an idea about operator precedence.

| Operator                                         | Description                                            |
|--------------------------------------------------|--------------------------------------------------------|
| ()                                               | Parentheses                                            |
| **                                               | Exponentiation                                         |
| +x, -x,~x                                        | Unary plus, unary minus, and bitwise NOT               |
| *, /, //,  %                                     | Multiplication, division, floor division, and modulus  |
| +, -                                             | Addition and subtraction                               |
| <<, >>                                           | Bitwise left and right shifts                          |
| &                                                | Bitwise AND                                            |
| ^                                                | Bitwise XOR                                            |
| |                                                | Bitwise OR                                             |
| ==,  !=, >,  >=, <, <=, is, is not, in, not in   | Comparisons, identity, and membership operators        |
| not                                              | Logical NOT                                            |
| and                                              | AND                                                    |
| or                                               | OR                                                     |


> Note:  If two or more operators have the same precedence, the expression looking from left to right

## String Operators

In the previous article, we talked about string data type in Python. Now, we are going to look at what are the operators which can be used for string. First, let’s look at string concatenation and string repetition. 

```python
noun = "Python"
verb = "is"
adjective = "awesome."

print(noun + verb + adjective )# string concatenation
print(noun * 5) # string repetition
```

Above the code block, there are three string variables and two print statements. In the first print statement, we can see string concatenation. For string concatenation, you can simply use the `+` sign. At this moment, we combined three strings. You can combine any number of strings using the `+` sign. Here, it returns a single string to us. The second print statement gives the value of the variable `noun` five times. That is called string repetition. For string repetition, first, mention the string variable that you want and then put the `*` sign and putting how many times you want to repeat the string. Also, this operation gives a single string.

Basically, strings are sequences of characters. You can access those characters by the slice operator in Python strings. For that, we are using square brackets. Like below,

```python
text = "Python is a very cool language."

print(text[0]) # get first character
print(text[5]) # get sixth character
print(text[-1]) # get last character
```

We have simple text that stored in `text` variable. In the first print statement, you can access the first element of the character sequence. As we know,  in programming we are counting from zero in most places. And in the last print statement, you can see a negative one in there. It means the last character of the string. If you need to access the last character, you can use this. But, remember you can only get that characters, you can not change them. Because strings are immutable data-type. Immutable means we can not update the object type over time. 
Also, the values of the immutable object remain permanent and unchangeable. This is the reason why we are not changing characters in strings. Suppose, you want to select a range of characters in a string. How do we do that? You can do it like this.

```python
text = "Python is a very cool language."
print(text[0:4:2]) # output - Pt
```

Above, we are using range slicing in Python. In the square brackets, you can put three parameters, first one is the start position of the range, the second is end position of the range and the last one is the step of the range its default value is one. The third one is not necessary, but if you want, you can use it.

I think, now you have an idea of operators in Python. In our next article, we will cover data collections in Python language. See you in the next article.

