---
sidebar_position: 3
---

# Lists
A List is a collection who is ordered and changeable, allows duplicate members.

## Create a List
The following lists hold different types of data:

```python title="my-python-app/lists.py"
numbers = [1, 2, 3, 4, 5]
fruits = ['Apples', 'Oranges', 'Grapes', 'Pears']

```
You can also use other data types like null, undefined, and so on.

You can also use the constructor to create a new list:
```python title="my-python-app/lists.py"
# Use a constructor
numbers2 = list((1, 2, 3, 4, 5))
```

## Get values from a list
Lists are ordered, so each element inside a list is represented by an index, which is how you can access it:
```python title="my-python-app/lists.py"
# Get the first value
print(fruits[0]) # Apples

# Get the second value
print(fruits[1]) # Oranges
```
Indexes are zero-based, so the first item has an index of 0, second has an index of one, and so on.

## List Methods
List methods are used to manipulate and get information about a list. Examples are appedning an item to a list, removing an item and reversing the list. 

An example of a list method is `append()`, which is used to add an element to the end of a list:

```python title="my-python-app/strings.py"
fruits.append("Banana") # Adds Banana to the fruits list

# Capilaize string
print(s.capitalize()) # 'Hello world'
```

There are dozens of other methods for perfroming various actions on a string.

They're basically used the same way - it's just . followed my the method. For some, you have the option to pass paramters to customize the function.

Here are some of the methods and their use:

```python title="my-python-app/strings.py"
# Get length
print(len(fruits))

# Remove "Grapes" from list
fruits.remove('Grapes')

# Insert 'Strawberries'into position three in the list
fruits.insert(2, 'Strawberries')

# Change the first value to 'BlueBerries'
fruits[0] = 'Blueberries'

# Remove with pop
fruits.pop(2)

# Reverse list
fruits.reverse()

# Sort list
fruits.sort()

# Reverse sort
fruits.sort(reverse=True)

print(fruits)

```