---
sidebar_position: 2
---

# Strings
Strings in Python are surrounded by either single or double quotation marks. They are used to represent textual characters such as name, place or animal. 

Let's look string formatting and some string methods.

## String Concatenation
You can join (or concatenate) two or more strings togther, and also join a string to another data type like an integer:
```python title="my-python-app/strings.py"
name = "Kingsley"
age = 26

# concatenate
print('Hello, my name is ' + name + 'and I am' + str(age))
```
We had to convert the age from integer to string using str() method.

If you run the code with `python3 strings.py`, you'll get: 

> *Hello, my name is Kingsley and I am 26*

There's better ways to insert variables into strings, and you'll see them in the next section.

## String Formatting
### Arguments by position
Another way to format strings in Python is by using the `format()` method:

```python title="my-python-app/strings.py"
print('Hello, my name is {name} and I am {age}', format(name=name, age=age))
```
So the curly braces `{}` are basically placeholders for whatever variables we add in the format() method. The method injects the variable into the string.

If you run the code with `python3 strings.py`, you'll get: 

> *Hello, my name is Kingsley and I am 26*

### Using F-Strings
F-String is the most convenient way to format stings in Python:

```python title="my-python-app/strings.py"
print(f'Hello, my name is {name} and I am {age}')
```
That's all - you don't need an extra method or plus symbols. Running the code gives you the same result as the last two.

> *F-Strings are only avaibale in Python 3.6 and above. So you might not be alble to use it in an older Python version.*

## String Methods
String methods are used to manipulate and get information about strings. Examples are capitalizing a string, getting the length of a string, returning a string subset, and so on.

An example of a string method is `capitalize()`, which is used to capitalize the first word in a string:

```python title="my-python-app/strings.py"
s = 'hello world'

# Capilaize string
print(s.capitalize()) # 'Hello world'
```

There are dozens of other methods for perfroming various actions on a string.

They're basically used the same way - it's just . followed my the method. For some, you have the option to pass paramters to customize the function.

Here are some of the methods and their use:
```python title="my-python-app/strings.py"
# Makes all uppercase
print(s.upper())

# Makes all lowercase
print(s.lower())

# Swap case, e.g. from 'Kingsley Is great' to 'kINGSLEY iS GREAT'
print(s.swapcase())

# Get the length, i.e. the number of charaters in a string (whitespaces included)
print(len(s))

# Replace, in this case, world with everyone
print(s.replace('world', 'everyone'))

# Count the number of a given character (e.g. h) inside a string
sub = 'h'
print(s.count(sub))

# Returns true if a string starts with a given value (e.g. hello)
print(s.startswith('hello'))

# Returns true if a string ends with a given value (e.g. hello)
print(s.endswith('d'))

# Takes a string and turns it into a list
print(s.split())

# Find position
print(s.find('r'))

# Is all alphanumeric
print(s.isalnum())

# Is all alphabetic
print(s.isalpha())

# Is all numeric
print(s.isnumeric())
```


