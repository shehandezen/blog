---
title: Lists in Python
description: In this blog, we will cover lists in Python language. 
date: 2023-04-07
image: cover.png
categories:
    - Python
tags:
    - Lists
    - List Slicing
    - List Concatenation

--- 

Well, today we are going to dive deep into data collections in Python language. We will cover what is the meaning of data collection and also learn list data type in Python. First, we need to understand what is the meaning of data collection. By now you know about text and numeric data types in Python. Whereas, we could store one value. But sometimes, we need to store multiple values in one single variable. Then, you can use data collection. Simply, data collection means that can store more than one value in a single variable. Also, those are naming as container data types. Python has many container data types such as lists, tuples, dictionaries, and sets. Now, let’s talk about the list container data type.

## Lists in Python

Lists in Python are a mutable and changeable sequence of elements. Also, lists are a type of data structure in Python. Simply, you can define a list by using square brackets `[]`. We can put data into the list by separating it by commas. Also, we can put any kind of data type into the list such as string, integer, float or even a list.  That is the structure of the list. You can see it on the below code,

```Python
x = ['savindu',20,['AI',' Cloud computing'], 56.2] # define a list
```

### Accessing a list

After, defining a list we can access each element in the list. For that, we can use the variable name of the list and the index of the element inside the square brackets. Also, indices of the lists are starts from zero like strings.  Here, you can access the elements as well as update those values. Because lists are mutable object type of Python.

```python
x = ['savindu',20,['AI','Cloud computing'], 56.2] # define a list


print(x[0]) # access the first element in the list.
print(x[-1]) # access the last element in the list.


x[1] = 19 # updating a element in the list
```
### Appending to a list

Suppose, you want to add new items to the list. For that, we can use a built-in function in the list object called `append()`. When using the `append()` function, first,  mention the variable name of the list and put the `.` after the variable name and then you can put the `append()` function. Finally, you can put the value you desired to add to the list inside the parentheses. The `append()` function adds our value to the end of the list. Like below,

```python
x = ['savindu',20,['AI','Cloud computing'], 56.2] # define a list
# Appending a list
x.append('shehan')
```

### Deleting a Value from a List

If you want to delete an element in the list. Simply, you can use the `remove()` built-in function in the list object, just like the `append()` function. Here, you can pass the value that you need to remove inside the parentheses. Suppose, you want to remove the third element of the above example list. You can do this like the below code,

```python
x = ['savindu',20,['AI',' Cloud computing'], 56.2] # define a list
# appending a list
x.remove(['AI',' Cloud computing']) # remove the third element in the list.
```

And also, we have another option. You can use the `del` keyword. When using the `del` keyword, we can remove an item using its index.

```python
x = ['savindu',20,['AI','Cloud computing'], 56.2] # define a list
# appending a list
del x[2] # Remove the third element in the list.
```

### Multi-dimensional List

As we know, lists are a type of data collection. Also, we know, we can put any data type value to the list. As I mentioned before, we can put even a list in the list. When there is a list of lists, we call that list a multi-dimensional list or a nested list.

```python
x = [[1,2,3],[4,5,6],[7,8,9]] # multi-dimensional list
```

###  List operations

Now, we are going to talk about list operations in Python such as getting the length of the list, list concatenation, list repetition, list iteration, and slicing. The `len()` function can be used to get the length/size of the list. That is  a built-in function in Python. Also, This function can be used to get the length of a string.

```python
x = [1,2,3,4,5,6,7,8,9,0] # define a list
print(len(x)) # using len() function
```

We can do concatenation and repetition in lists by using the `+` sign and the `*`  sign like strings. 

```python
x = [1,2,3,4,5]
y = [6,7,8,9,0]
z = ['Hello']


print(x + y) # list concatenation
print(z * 5) # list repetition
```

We also can do membership operations in lists by using `in` or `not in` keywords. You can use it to check if a value does exist in a list. Like below,

```python
print(3 in [1,2,3]) # using the membership operator for a list
```

Now, let’s talk about iteration in a list. The iteration means going through the list one element at a time. For that, You use the `for` loop like below, 

```python
x = [1,2,3,4,5,6,7,8,9]


for i in x:
    print(i) # Print all the elements one by one

```

Finally, we learn about list indexing and slicing. As mentioned before, the index of the lists starts with zero. And also, lists have negative indices. You can clarify it by the below table,

|                | [ a,  |  b, |  c ] |
|----------------|-------|-----|------|
| Positive Index |   0   |  1  |  2   |
| negetive Index |  -3   | -2  | -1   |

You can do slice operation just like those used in strings. When using the slice operator, first mention the variable name of the list and second, you can pass three values separated by a colon inside the square brackets. The first value is the start index, the second is the end index and the third is the step value. You can see it by the below code,

```python
x = [1,2,3,4,5,6,7,8,9]


print(x[:2]) # slice first element to third element
print(x[3:]) # slice fourth element to last element
print(x[1:5:2]) # slice second element to sixth element two by two
```

Are you notice a special thing in the above code? If you want to select zero index in the start position, you won’t mention it, you can keep it blank. And also, if the end position is the last item, you won’t mention it, you can keep it blank.

lastly, you have an idea of lists in Python. In our next article, we will cover tuples in Python language. Then, Goodbye!



