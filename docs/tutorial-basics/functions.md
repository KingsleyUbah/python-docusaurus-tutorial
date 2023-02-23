---
sidebar_position: 7
---

 # Functions
 A function is a block of code which only runs when it is called. In Python, we do not use curly brackets, we use indentation with tabs or spaces.

 ## Create a function
 To define a function, we use the `def` keyword:
 ```python title="my-python-app/function.py"
# Define the function
def sayHello(name):
    print(f'Hello {name}')

# Invoke the function
sayHello('Sam')
 ```
 If you run the code above, you'll get the following output:
 > *Hello Sam*

If the name 'Sam' was not passed to SayHello() in invocation, we'd have gotten a ''missing required argument" error.

We can get around this by setting a defualt parameter:
```python title="my-python-app/function.py"
def sayHello(name='Sam'):
    print(f'Hello {name}')

sayHello('Jake')
```
So if a name is passed as argument on invocation, as in the above example, then that name is used. So the above code outputs:
> *Hello Jake*

But if no argument is provided, it uses the default name, Sam.

## Return values
Usually, you're going to be returning something from your function. 

```python title="my-python-app/function.py"
# Return values
def getSum(num1, num2):
    total = num1 + num2
    return total
```

The above function returns the sum of two numbers when invoked:
```python title="my-python-app/function.py"
print(getSum(5,5)) # 10
```