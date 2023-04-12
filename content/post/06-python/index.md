---
title: Sets in Python
description: In this blog, we will deep dive into sets in Python. 
date: 2023-04-12
image: cover.png
categories:
    - Python
tags:
    - Sets
    - Sets operations
    

--- 

Hello friends! Today, we will cover many aspects of the Set container data type in Python. By now, we have learned about two container data types such as lists and tuples. In this article, we will learn the meaning of the set data type, how to create a set and many more. In previous articles, we covered lists and tuples; those data types had indices but sets had no indices. Simply, a set is a collection of unique, unordered, and unindexed data. The elements of a set can be of any data type. If we need to store unique values, we can use sets in Python. For example, if you want to store information about employee id, you can use sets because employee id does not duplicate. 

## Create a Set

Now, let’s look at how to create a set in Python. Normally, we can use curly braces `{}` to define a set. The data can be put inside the curly braces separated by commas. Like below,

```python
ids = { 11220, 556622, 884455, 996632} # define a set

print(type(ids)) # <class 'set'>
print(ids) # print the set
```

## Access elements in a Set

As I mentioned before, the set is the unindexed container data type. Therefore, we can not access the elements of a set by using an index. So, how do we access elements of a set? We can do it by looping through the set. Like this,


```python
ids = { 11220, 556622, 884455, 996632} # define a set

for i in ids:
    print(i) # print element by element in the set
```

## Add, Delete and update elements in Sets

Also, The sets are mutable objects in Python. You can update, insert or delete data in a set if you want. First, let’s look at how to add an item to a set. For that, we can use the `add()` function in the set object. We can pass only a string, an integer, a float, a complex number, and a boolean value. Here, our new item takes the first position in the set. 

```python
ids = { 11220, 556622, 884455, 996632} # define a set

ids.add(255588) # add new item to the set
```

In that method, we can add a single item. Suppose, you want to add multiple items to the set. Just like that time, we can use another function in the set object called the `update()` function. In the `update()` function, we can pass any data collection type as the argument of the function. Like this,

```python
ids = { 11220, 556622, 884455, 996632} # define a set

ids.update([885544, 66244, 887755]) # add multiple items to the set
```

If you want to delete an item in the set, there are three functions available such as `remove()`, `discard()`, and `pop()`. The `remove()` function can use if we need to remove a specific item in the set. Here, if the item does not exist in the set, python gives an error. But, when using the `discard()` function, python will not raise an error even if the item is not present in the set. The `pop()` function can use to remove a random item in the set. You can see below how to use that functions.


```python
ids = { 11220, 556622, 884455, 996632} # define a set

ids.discard(556622) # remove an specific item
ids.remove(996632) # remove an specific item
ids.pop() # remove random item in the set
```

## Length of the Set

To get the length of the set, simply, we can use the `len()` function. 


```python
ids = { 11220, 556622, 884455, 996632} # define a set

print(len(ids)) # get length of the set
```

## Set Operations

If you know about sets in mathematics, there are many operators for the sets to perform special operations like union, intersection, difference etc. Also in Python, we can do like that operations in a set. First, let’s understand the meanings of that operations. The union operation is all the elements in the given sets. The `union()` function is used to do union operations in Python. The intersection operation gives the common elements in given sets. To do that, we can use the `intersection()` function in Python. To understand the difference operator, let’s think we have two sets. The difference is the list of elements that are available in one set but that are not present in another set. The `difference()` function can be used to get the difference between two sets. Now, we can try those on Python.


```python
x = {1,2,3,4,5,6,7,8,9}
y = {2,4,6,8,0}

# Union
x.union(y) # {0, 1, 2, 3, 4, 5, 6, 7, 8, 9}

# Intersection
x.intersection(y) # {8, 2, 4, 6}

# Difference
x.difference(y) # {1, 3, 5, 7, 9}
```

I think now you have some knowledge about the sets in Python. You can try the above code blocks yourself on your favourite IDE.  Goodbye, friends! 

