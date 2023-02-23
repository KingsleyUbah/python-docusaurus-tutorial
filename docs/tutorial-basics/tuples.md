---
sidebar_position: 4
---

# Tuples
A Tuple is a collection which is ordered and unchangeable. Allows duplicate members.

## Create a Tuple
To create a tuple, you simply create a prenthesis with the different elements:
```python title="my-python-app/tuples_sets.py"
# Create tuple
fruits = ('Apples', 'Oranges', 'Grapes')

# Using a constructor
fruits2 = tuple(('Apples', 'Oranges', 'Grapes'))
```

If you're assigning a single value, you need to add a trailing comma:
```python title="my-python-app/tuples_sets.py"
fruits2 = ('Apples',)
```

## Get values from a Tuple
Elements inside a tuple are accessed by their index:
```python title="my-python-app/lists.py"
# Get the first value
print(fruits[1])
```

## Can't change a value
Once a tuple is created, it can't be modified, so this'll not work:
```python title="my-python-app/lists.py"
# Can't change value
fruits[0] = 'Pears'
```
If you run the code, you'll get the following error message:

> *TypeError: 'tuple' object does not support item assignment*

This makes Tuple the perfect storage for constant, non-changing data(e.g. PI).

## Delete a Tuple
To delete a Tuple, simply use the tuple next to the `del` keyword:
```python title="my-python-app/lists.py"
del fruits2

print(fruit2)
```
If you run the following code, you'll get the following error message:

> *NameError: name 'fruit2' is not defined*

