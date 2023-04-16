---
title: Loops in Python
description: In this blog, we will cover loops in Python language. 
date: 2023-04-16
image: cover.png
categories:
    - Python
tags:
    - for loop
    - while loop
    - break keyword
    - continue keyword
    - pass keyword
    

--- 

Hi everyone! Today, we are going to talk about an interesting topic called loops in Python. When you write a computer program, you might be had to write the same block of code repeatedly. For just-like moments, we can use loops. The loop means a block of code executes several times or till completing a special condition. In programming, we have two methods for looping a code block. They are the `for` loop and `while` loop. 

## `for` loops

 The `for` loop is normally used for executes a code block a specific number of times. In Python, The `for` loops are mostly used to iterate data sequences. Ok now, let's look at how to use the `for` loop in Python. The syntax of the `for` loop is,

```python
for value in sequence:
    # body of the loop
```

> Note: you must indent the body of the loop to the `for` loop statement.

## `range()` function

In the loops, the `range()` is so useful. Because we can generate a sequence of numbers by using that function. For that, we need to pass three arguments into the `range()` function. They are start, end and step. The start is the starting position. The end is the ending position. And also, the step is the stepping value. The default value of the step is one. Let’s try it.

```python
numbers = range(0,9,2) # generate numbers between 0 and 9 two by two.

for i in numbers:
    print(i)
```

> Remember the number of en position does not include that sequence.

The `range()` function can use to generate a list. Like this,

```python
numbers = list(range(0,9,2)) # generate a list of numbers between 0 and 9 two by two.
print(numbers)
```

## `while` loops

Well, The `while` loop is used to repeat a code block as long as a special condition is true. Below, you can see the syntax of the `while` loop in Python. 

```python
while condition:
    # loop body
```

If you are using the `while` loop. You need to be concerned about a special thing. Initializing, incrementing and other actions on the elements in the conditions should be taken care of by the programmer.  Let’s clarify it with an example. 

```python
count = 0 # initialising a count

while count < 5:
    print(count)
    count += 1 # increment count by one
```

Here, we initialized a variable called `count`. And in the body of the loop, we increased the `count` variable by one. If we do not do it, the `while` loop does not finish because its condition is always `True`. 


## Nesting of loops

Alright! You can nest a loop inside another loop.  We can nest a `for` loop inside a `while` loop or a `while` loop inside a `for` loop. And also, you can nest the `for` loop in a `for` loop and the `while` loop in a `while` loop. Like below,

```python
count = 0 # initialising a count

while count < 5:
    for i in range(0,5):
        print(count, i)
     
    count += 1 
```

## Loop manipulation

Sometimes loop manipulation is necessary to take action within a structure that is different to the normal operation. For that, python has provided three keywords. They are `break`, `continue` and `pass`. 

## `break` keyword

The `break` keyword is used to terminate a loop suddenly. You can see it in this example,

```python
count = 0 # initialising a count

while count < 5:
    print(count)

    if count == 4:
       break # use the break keyword
    count += 1
```

>  Note: The `break` keyword within a loop should always be put inside an `if` statement. Otherwise, it will break in the first iteration.

## `continue` keyword

The `continue` is used inside a loop to skip the rest of the loop body in the current iteration. It will continue with the next iteration of the loop. We can use the `continue` keyword to jump to the loop control statement when we want. As the `break` keyword, you should put the `continue` keyword inside an `if` statement. Otherwise, it will never execute code after the `continue`. 

```python
for i in range(5):
    if i == 3:
        continue
    print(i)
```

## `pass` keyword

The `pass` is used when we have a loop that is not implemented yet. 

```python
while True:
    pass
```

## `else` with loops

Well, now we will look at using `else` with loops. Python allows using `else` with loops. The `else` code block is executed when the loop is finished. For example,

```python
count = 0
while count < 5:
    print(count)
    count += 1
else:
    print("loop finished.")
```

Today we talked about loops in Python. In the next article, I will cover functions in Python. Until then, Goodbye! 
