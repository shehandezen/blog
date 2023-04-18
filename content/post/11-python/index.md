---
title: Functions in Python
description: In this article, we will learn functions in Python. 
date: 2023-04-18
image: cover.png
categories:
    - Python
tags:
    - functions
    - positional arguments
    - named arguments
    - packed arguments
    - keyword arguments
    
--- 

Hi there! By now, we covered many topics in Python such as data types, loops, and data collection. Today, we are going to learn about functions in Python. Let’s start this. In programming, a function is a block of code that we can reuse over and over again in our program. Sometimes, we have to do the same job in different places in our program. At this time, we can use functions. So, we can write readable and maintainable code by using functions. Also, the functions help to reduce the complexity of our code. 

Ok, now, let’s look at how to define a function in Python. This is the syntax of the functions.

```python
def function_name(arguments):
    # function body
    pass
```

Defining a function is not enough to execute the function body. For that, we need to call that defined function in the main program by its name. This is the syntax,

```python
function_name(arguments)
```

Let’s try that by example.

```python
# define a function
def greet():
    print(“Welcome !!!”)
 
# call the function
greet()
```

> Remember, you need to define the function before calling the function. Otherwise, python gives an error.

Well, now you know how to define and call a function. 

Now, we are going to learn about arguments in a function. They are many types of arguments such as positional arguments, named arguments, packed arguments and keyword arguments. Now let’s look at each one. 

## Positional Arguments

The positional arguments maintain a specific order. You need to pass positional arguments in that order. Otherwise, the function may give unexpected results. Also, we must pass a number of arguments that equals the  number of arguments introduced when defining the function. It is a rule of using functions in Python. If you do not follow it, python gives an error. Let’s try it,

```python
# define a function
def add(num_1, num_2):
    print(num_1 + num_2)
 
# call the function
add(2,8)
```

## Named Arguments

Sometimes, you might not remember the order of the arguments. Then, you can use named arguments. The named arguments are not ordered. We can assign values to the arguments by their names when calling the function.  Like this,

```python
# define a function
def get_details(name, age):
    print(name, age)
 
# call the function
get_details(name = "Savindu", age = 20)
```

Here also, you should follow the rule that I mentioned before. 

Suppose, you need to pass three arguments, but you do have not enough data. At this moment, we can use default values for functions. Like this,

```python
# define a function
def get_details(name, age = "unknown"):
    print(name, age)
 
# call the function
get_details(name = "Savindu")
```

## Packed Arguments

You know the `print()` function can get any number of arguments. Now let’s look at how to do it to our functions. For that, we can use packed arguments. Like this,

```python
# define a function
def get_details(*args):
    print(args)
 
# call the function
get_details(20, 8.5, 96, "text")
```

Here, you can put the `*` sign before the argument name, when you define a function. Then you can pass any number of arguments into the function. Actually, all the arguments that we passed to the function are packed into a tuple. You can access the arguments just like accessing elements in the tuple. Like below,

```python
# define a function
def get_details(*args):
    print(args[0])
    print(args[2])
 
# call the function
get_details(20, 8.5, 96, "text")
```

## Keyword Arguments

Suppose, the function has many arguments but you do not need to use all arguments. For that, python introduces keyword arguments. By using keyword arguments, we can pass arguments our desired only. To define keyword arguments, you can put double `*` signs before the argument name when you define a function.  You can understand that in the below example,

```python
# define a function
def get_details(**args):
    print(args)
   
 
# call the function
get_details(name = "savindu", age = 20, city = "Colombo")
```

Here, the arguments are converted into a dictionary. Therefore we can access those arguments just like accessing elements of a dictionary.

```python
# define a function
def get_details(**args):
    print(args['name'])
    print(args['city'])
   
 
# call the function
get_details(name = "savindu", age = 20, city = "Colombo")
get_details(name = "shehan", city = "Kalutara")
```

Also, we can use packed arguments with keyword arguments. For that, you should remember one thing. You need to pass packed arguments before the keyword arguments. You can see it in this example.

```python
# define a function
def get_details(*params, **args):
    print(params)
    print(args)
   
 
# call the function
get_details(50, 84, name = "savindu", age = 20, city = "Colombo")
get_details(8, 56, 85, name = "shehan", city = "Kalutara")
```

## `return` keyword

So far, we used the `print()` function to see the result of the function. We can use the `return` keyword to get result of the function. 

```python
# define a function
def add(*params):
    total = 0
    for i in params:
        total += i
    return total
 
# call the function
sum = add(12, 85)
print(sum)
```

## Docstring in functions

The docstring is a string used to document a function. The docstring is added as the first statement in the body of a function. These need to be within quotation marks and the recommended convention is to use triple quotes. You can get docstring by `__doc__`.

```python
# define a function
def add(*params):
    """ Return sum of the given numbers """
    total = 0
    for i in params:
        total += i
    return total
 
print(add.__doc__)
```

I think now you have some knowledge about the functions in Python. You can try the above code blocks yourself on your favourite IDE. Goodbye, friends!