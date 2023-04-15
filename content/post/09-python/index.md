---
title: If statement in Python
description: In this blog, we will cover decision-making statements in Python language. 
date: 2023-04-15
image: cover.png
categories:
    - Python
tags:
    - if
    - if...else
    - if...elif...else

--- 

In this tutorial, we will learn decision-making statements in Python. That means we will look at `if` statements. We can create decision-making programs using that statements. The `if` statements are used if the program meets the programmer-defined condition and then executes a code block. Python has three forms of the `if` statement. They are the `if`, `if … else`, and `if … elif … else`.  

## `if` statement

First, let's look at a single 'if' statement. In this statement, the 'if' evaluates the condition of the 'if' statement, if the evaluation is 'true', the body of the 'if' is executed by Python and if the evaluation is `False`, the code block is skipped by Python. Now, let’s clarify that using the below example,

```python
if(25 > 5):
    print("The condition is True.") # Body of the if statement

print("program end")
```

> Remember indentation is most important in Python. Because python recognizes code blocks by indentation.  

## `if...else` statement

Now, we add the `else` keyword to the `if` keyword. The single `if` statement can only execute the code block when the condition is `True`. By that, we can execute code blocks when the condition is `True` as well as `False`. If the condition is `True`, python executes the code block which is inside the `if`. And if the condition is `False`, python executes the body of the `else`.  

```python
if(2 > 5):
    print("The condition is True.") # Body of the if
else:
    print("The condition is False") # Body of the else

print("program end")
```

## `if...elif...else` statement

Alright! Now we will learn the third form of the `if` statement. The `if … elif … else` is used to evaluate more than one condition. The evaluation of the `if` statement is `False`, we can evaluate another condition by `elif`. In the below, we can see how it use,

```python
if(2 < 5):
    print("The condition is True in the if.") # Body of the if
elif(5 < 8):
    print("The condition is True in the elif.") # Body of the elif
else:
    print("The conditions are False") # Body of the else

print("program end")
```

## Nested `if` statements

Also, we can nest `if` statements in another `if` statement. Like below,

```python
if(2 < 5):
    print("The condition is True in the if.") # Body of the if
    if(2 < 5):
        print("The condition is True in the  nested if.") # Body of the if
    elif(5 < 8):
        print("The condition is True in the elif.") # Body of the elif
    else:
        print("The conditions are False") # Body of the else

print("program end")
```

> Remember, when using nested `if` statements. You need to maintain indentation correctly.

Well, now we are coming to the end of today’s article. Until we meet on next article. Goodbye, everyone!  
