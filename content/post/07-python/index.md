---
title: Dictionaries in Python
description: In this article, we are going to cover dictionaries in Python. 
date: 2023-04-13
image: cover.png
categories:
    - Python
tags:
    - Dictionaries 
    - Dictionaries operations
    

--- 

Hi there! Now, we will cover our last data collection type called the dictionary data type. In this article, we will cover what is a dictionary in Python, how to define a dictionary, dictionary operations and many more. 

## Create a Dictionary

First of all, let’s understand what is the dictionary. The dictionaries are a collection of key-value pairs. The definition of the dictionary is an ordered, changeable, indexed data collection type in Python. And also, dictionaries do not allow storing duplicate values. The dictionaries are created by using curly braces `{}` and have keys and values. 

```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary
```

## Access elements of a Dictionary

Here, you can see how we create a dictionary. The main advantage of the dictionary we can quickly access to data is required. Because dictionaries consist of programmer-defined indices called keys, not consist of numerical indices. You can access the values of a dictionary using that keys. For that, you can mention the variable name of the dictionary and put the key inside the square brackets like below,

```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary
print(x["Name"])# access the first value using "Name" key
```

Also, we have another method to access values in a dictionary. The `get()` function can be used to get value according to the key. You can pass the key within the parentheses in the `get()` function.

```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary
print(x.get("Country")) # access value using get() function
```

We can get a list of the all keys in the dictionary using the `keys()` function. And also, the `values()` function can use to get a list of all the values in the dictionary. Now, let’s try those functions,

```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

print(x.keys())# list of all the keys
print(x.values()) # list of all the values
```

The dictionary object has another useful function called the `items()`. That function is used to convert a dictionary into a list of tuples. 

```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

print(x.items()) # Output - [('Name', 'Savindu'), ('Age', 20), ('Country', 'Sri Lanka')]
```
# Operations of Dictionaries
## Add an Element

Alright! Now we are going to learn about operations in dictionaries such as adding elements, updating a dictionary, removing elements, and dictionary iteration. First, let’s look at how to add elements. 

```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

x["City"] = "Kalutara" # adding new element
```

## Update an Element

And also, we can update an element like the below code,

```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

x["Name"] = "Savindu Shehan" # updating first element
```

We can do the above operation using the `update()` function. Here, we have two methods. First is passing the updated elements as a dictionary inside the parenthesis to update the dictionary. The second is updating the dictionary by assigning.


```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

x.update({"Name": "Savindu Shehan", "Age": 19}) # Update the dictionary by passing a dictionary
x.update(Age = 20) # update the dictionary by assigning
```

## Delete an Element using `del` keyword

To remove an element, we have many methods. First, let’s look at how to do it using the `del` keyword.

```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

del x["Age"] # delete an element
```

## Delete the Dictionary

If you want to delete the entire dictionary, you can do it like this, 

```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

del x  # delete a dictionary
```

## Delete an Element

The `pop()` function and the `popitem ()` function can use to remove an element in the dictionary. The `pop()` function can use to remove a specific element in the dictionary. And the `popitem()` function is used to remove the last element of the dictionary. 

```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

x.pop("Age") # remove an element
x.popitem() # Remove the last element
```
## Clear the Dictionary

Suppose, you need to remove all the elements in the dictionary. For that, the dictionary object has a `clear()` function. You can clear the dictionary using that function.

```python
x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

x.clear() # clear the dictionary
```
## Iterating through a Dictionary

Now, we will learn about iteration operations in a dictionary. We have four methods to iterate through a dictionary.

1. Using a for loop
    ```python
    x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

    for i in x:
        print(i, x[i])
    ```

2. Using the `enumerate()`
    ```python
    x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

    for i in enumerate(x.items()):
        print(i)

    # output
    # (0, ('Name', 'Savindu'))
    # (1, ('Age', 20))
    # (2, ('Country', 'Sri Lanka'))
    ```
Here, the `enumerate()` function is that it returns a tuple with the counter and value. We need to pass `x.items()` inside the parenthesis.


3. Using the `items()` method in the dictionary Class.
    ```python
    x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary


    for key, value in x.items():
        print(key, value)
    ```

4. Using list comprehension. 
    ```python
    x = {"Name": "Savindu", "Age": 20, "Country": "Sri Lanka"} # define a dictionary

    y = [(i, x[i]) for i in x]

    # Output
    # [('Name', 'Savindu'), ('Age', 20), ('Country', 'Sri Lanka')]
    ```

Now, we have come to the end of today’s article. Lastly, we should concern about which times not to use a dictionary. 

1. For storing data that shouldn’t be modified.
2. When resource (memory) usage is a concern. 

By now, we have covered data collection types in Python. In the next article, we will look at data collection type comparison and type conversion. Goodbye! 





