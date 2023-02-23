---
sidebar_position: 6
---

# Dictionaries
A Dictionary is a collection which is unordered, changebale and indexed. It's comprised of proprties, which appear in name: value pairs. It doen't acceopt duplicate members.

## Create a dictionary
Here's a dictionry representing a person:
```python title="my-python-app/dictionaries.py"
# Create dict
person = {
    'first_name': 'John',
    'last_name': 'Doe',
    'age': 30
}
```
So the person has three properties - `first_name`, `last_name` and `age`.

You can also create an object using the constructor:
```python title="my-python-app/dictionaries.py"
# Use constructor
person2 = dict(first_name='Sara', last_name='Williams')
```
## Get a value from a dctionary
You access a value in a Python dictionary by it's property name:
```python title="my-python-app/dictionaries.py"
print(person['first_name'])
```
This outputs the value of `first_name`, which is 'John'.

You can also use the `get()` method to access values:
```python title="my-python-app/dictionaries.py"
print(person.get('last_name'))
```
This outputs 'Doe', the last name.

## Add a new proprty
You add a new property in a dictionary in key/value pairs:
```python title="my-python-app/dictionaries.py"
person['phone'] = '555-555-5555'
```
This creates a new phone key in the dictionary and assigns it '555-555-5555'. However, if the phone property already exists, it simply replaces its value with the new one.

## Remove a property
To remove a propery from a dictoary, use the del keyword and specify the property to delete:
```python title="my-python-app/dictionaries.py"
del(person['age'])
```
This removes the age field from the dictionary completely. You can also use the `pop()` method to achieve the same thing:
```python title="my-python-app/dictionaries.py"
person.pop('phone')
```

