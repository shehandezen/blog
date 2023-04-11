---
title: Tuples in Python
description: In this blog, we will cover tuples in Python. 
date: 2023-04-11
image: cover.png
categories:
    - Python
tags:
    - Tuples
    - Tuple operations
    

--- 

Hey guys, in this article, we are going to learn about another data collection type in Python called Tuples. Today, we will cover the meaning of the tuples and how to use them in Python. If you know about relational databases, you might hear a term called a tuple. In the databases, a tuple is one single record of a table. It maintains specific order to store values according to the table header. In Python, The tuples are a sequence of an ordered collection of elements. Once, a tuple is created, it can not change its values because tuples are immutable data type.

## Define a Tuple

The structure of the tuple is the comma-separated sequence of values inside the parenthesis `()`.  The tuples can consist of different data types like strings, integers, lists etc. Also, a tuple may include in another tuple. When a tuple consists of other tuples, we called that tuple a nested tuple. You can see it in the below example code,

```python
my_tuple = (11, "Savindu", "Shehan", 20, "Sri Lanka", (1, "01117755446")) # Define a tuple
```

And also, we can define a tuple without parenthesis like this,

```python
my_tuple = 11, "Savindu", "Shehan", 20, "Sri Lanka",(1, "01117755446")# Define a tuple
print(type(my_tuple)) # <class 'tuple'>
```

## Access elements in Tuple

So, we use the `type()` function to get the data type of the given variable.  At this moment, we used the `type()` function to know `my_tuple` variable is exactly a tuple. After defining a tuple, we have access to each element in the tuple. We can access each element by its index. Also, the index of the tuples are start with zero, just like a list. Now, let’s try it.

```python
my_tuple = (11, "Savindu", "Shehan", 20, "Sri Lanka") # Define a tuple

print(my_tuple[0]) # access first element of the tuple
print(my_tuple[2]) # access third element of the tuple
```

The negative indices are also valid in the tuple. Therefore, We can use negative indices in tuples to access the elements. Just like this,

```python
my_tuple = (11, "Savindu", "Shehan", 20, "Sri Lanka") # Define a tuple

print(my_tuple[-1]) # access last element of the tuple
print(my_tuple[-3]) # access the third element from the end of the tuple
```

| Tuple            | 11, | “Savindu”, | “Shehan”, | 20, | “Sri Lanka” |
| Negative indices | -5  | -4         | -3        | -2  | -1          |

## Tuple Slicing

If you want to extract a part of the tuple, you can do it, just like lists. First, mention the variable name of the tuple and then pass the colon-separated three values inside the square brackets `[]`.  Suppose, we have to slice the `my_tuple` from 0 indexes to 2 indexes. Simply, we can slice it, just like the below, 

```python 
my_tuple = (11, "Savindu", "Shehan", 20, "Sri Lanka") # Define a tuple

print(my_tuple[0:3]) # slice the tuple 0 to 2
```

In the second code line, we sliced the `my_tuple`. If you look closely, you can notice one thing. Here, we want to slice 0 to 2 but we pass the end index as 3. because the end index is not included in the new sliced tuple. 

> Note: insertion, deletion and update are not possible in tuples. Because tuples are immutable data type.

## Tuple Unpacking

The tuple has a special feature called tuple unpacking. That means we can extract the content of the tuple into separated variables.

```python
my_tuple = (21, 52, "string") # define a my_tuple

x, y, z = my_tuple # extracting tuple
```

> Remember, you must put the number of variables that are equal to the length of the tuple on the left side. If we did not do it, python gives an error.  

## Tuple Operations

As in lists, we can do many operations like concatenation, repetition, and iteration in the tuples. You can try those like below,

```python
# tuple concatenation
x = (1,2,3,4,5)
y = (6,7,8,9,0)


print(x + y) # do tuple concatenation by + sign


# repetition
print(("Hello") * 3) # do tuple repetition by * sign


# iteration
for x in (1,2,3,4): # tuple iteration using for loop
    print(x)
```

Also, the membership operator is possible to use in tuples using the `in` keyword. By using it, we can check whether a value is available in a tuple.  

```python
my_tuple = (1,2,3,4,5)
print(3 in my_tuple) # use membership operator
```

The `len()` function can use to get the length of the tuple.

```python
my_tuple = (1,2,3,4,5)

print(len(my_tuple)) # get the length of the tuple
```

Well, I think now you have a good idea about tuples in Python. Now, you can use tuples for your Python programs. See you in the next article. 
