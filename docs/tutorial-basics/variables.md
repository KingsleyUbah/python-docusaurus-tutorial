# Variables
A Python variable is a reserved memory location to store values. 

- Variable names are case-sensitive (so `name` and `NAME` are different variables)
- The name must start with a letter or an underscore
- It can have numbers but cannot start with one

Just like in any language, there's a bunch of data types we can use, and we'll omly look at the more common ones.

## Create a variable
Here's a simple variable:
```python title="my-python-app/variables.py"
x = 1 # int
y = 2.5 # float
name = 'kingsley' # str
is_old = True # bool
```
With Python, semicolons are not needed. Also, when you declare a varible, there's no special symbol — just the variable and its value. You also don't have to declare the type, like int, String, etc.

### Multiple Assignment
You can assign mutliple values to their respective variables in one line:
```python title="my-python-app/variables.py"
x, y, name, is_old = (1, 2.5, 'kingsley', True)

print(x)
```
The print statement outputs the value of x (which is 1), when the file is executed.

To run the file, go to your terminal, cd into my-python-app, then run:
```bash
python3 variable.py
```
This outputs `Hello` on the terminal.

### Check the type of a variable
To check the type of data stored in variable, pass the variable to the `type()` function:
```python title="my-python-app/variables.py"
print(type(x))
```
If you run variables.py, you get `<class 'int'>` which says that x is an integer.

### Type casting
You can convert a value from one data type to another using a technique called **type casting**. 

Recall that the value of x is 1 (an integer). By wrapping it inside str() method, you convert it to a string — "1":
```python title="my-python-app/variables.py"

x = str(x) # converts to string
y = int(y) # converts to an integer
z = float(y) # converts to a float number

print(x) # outputs "1"
```
### Perform Basic Math
You can perform mathematics in Python variables. This includes addition, subtraction, multiplication, division, square root, and more.

```python title="my-python-app/variables.py"
a = x + y
b = x - y
c = x / y
d = x * y
```
That's all the basic things for variables. Up next, strings.