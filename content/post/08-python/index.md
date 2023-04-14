---
title: Summary of data collection in Python 
description: In this article, we will finish the data collection types in Python 
date: 2023-04-14
image: cover.png
categories:
    - Python
tags:
    - Type conparison 
    - Type conversion
    

--- 

Today’s article is a very short one. As I mentioned in the previous article, in this article, we are going to cover data collection types comparison and type conversion. First of all, we compare the list data type and the dictionary data type. Let’s do it.

## List Vs Dictionary

| List                                                    | Dictionary                                        |
|---------------------------------------------------------|---------------------------------------------------|
| Access using index                                      | Access using keys                                 |
| Collection of elements                                  | Collection of key-value pairs                     |
| Allow duplicate items                                   | No duplicate items                                |
| The indices of the list are integers starting from zero | The key of the dictionary can be of any data type |


In the above table, we compared the lists and the dictionaries. It can be useful to choose the best data type for your requirement. 

## Tuple Vs List

Well! Now, let’s compare tuples and lists. For that, we are concerned memory efficiency of the data type. See the below code block,

```python
import sys


my_list = [1,2,3,4,5,6,7,8,9]
my_tuple = (1,2,3,4,5,6,7,8,9)


print("Size of the list - ", sys.getsizeof(my_list)) # get the size of the my_list
print("Size of the tuple - ", sys.getsizeof(my_tuple)) # get the size of the my_tuple


# Output
# Size of the list -  128
# Size of the tuple -  112
```

I think you might understand what is the best memory-efficient data type. The tuples are more memory efficient than lists which means they consume less memory.

## Type Conversion

Alright! Now we go to the topic called type conversion. For type conversion between data collection types, we have four functions such as the `set()`, `list()`, tuple() and `dict()`. The `set()` function is used to convert any data collection type to the set data type. The `list()` is used to convert other data collection types to the list data type.  And also, the `tuple()` is used to convert other data collection types to the tuple data type. When we use the `dict()` function, we need to concern the data collection is consist of a list of lists, a tuple of lists, and a list of tuples. If not concern about this, sometimes Python gives an error. Let's try type conversion between data collection types.   

```python
my_list = [1,2,3,4,5,6,7,8,9] # List
my_tuple = (1,2,3,4,5,6,7,8,9) # Tuple
my_set = {1,2,3,4,5,6,7,8,9} # Set
my_dict = ([1,5],[8,6]) # a tuple of lists


print(list(my_tuple)) # tuple to list
print(tuple(my_list)) # list to tuple
print(set(my_tuple)) # tuple to set
print(dict(my_dict)) # a tuple of lists to dictionary
```

Ok guys, now we have finished data collection types in Python. You can practice data collections in Python. See you again in the next article.
