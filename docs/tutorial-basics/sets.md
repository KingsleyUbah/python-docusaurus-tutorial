---
sidebar_position: 5
---

# Sets
A Set is a collection which is unordered and unindexed. Have no duplicate members.

## Create a set
To create a tuple, you simply create a pair of curly brackets with the different elements:
```python title="my-python-app/sets.py"
# Create a set
fruits_set = {'Apples', 'Oranges', 'Mango'}
```

## Check item in a set
To check if a particuar item is present in a set, use the `in` operator:
```python title="my-python-app/sets.py"
# Check if Apple is in fruit_set
print('Apples' in fruits_set)
```
The above code returns `True` if Apple is in `fruit_set`, and `False` if not.

## Add item to a set
To add an item to a set, you use the `add()` method:
```python title="my-python-app/sets.py"
# Add Grape to set
fruits_set.add('Apples')
```
If an item already exists in a set, and you try to add it again, it won't return an error. It just doesn't add 'Apples' twice. So only one instance of Apple will be present in the set.


## Remove item from a set
To remove an item fron a set, you use the `remove()` method:
```python title="my-python-app/sets.py"
# Remove Grape from fruit_set
fruits_set.remove('Grape')
```
## Clear a set
Use the `clear()` method to clear a set entirely:
```python title="my-python-app/sets.py"
# Clear set
fruits_set.clear()
```
When you then do a print(set), it just gives you an empty set.

## Delete a set
You can also delete a set altogther by using the del keyword:

```python title="my-python-app/sets.py"
# Delete
del fruits_set
```
When you do a `print()` check on `fruit_set`, it'll return undefined.