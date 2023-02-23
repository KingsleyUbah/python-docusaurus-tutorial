# Modules
A module is basically a file containing a set of functions to include in your application. There are core python modules, modules you can install using the pip package manager (including Django) as well as custom modules

## Core modules
To import a mdoule, you use the import keyword:
```python title="my-python-app/modules.py"
import datetime

today = datetime.date.today()

print(today)
```
This outputs the current day. All we did was import the libary then we were able to use it's proprties and methods in our code.

Now instead of importing the whole datetime object, you can import just date:
```python title="my-python-app/modules.py"
from datetime import date

today = date.today()

print(today)
```
This gives the same output, but the code is smaller.

## Pip module
Before imporing a pip module, you need to install it. You use pip to install packages and manage dependenies in Python projects.

Let's say you want to use the camelCase package. First you install it with pip by running this command:
```python title="my-python-app/modules.py"
pip install camelCase
```
Once installed, you import the custom module:
```python title="my-python-app/modules.py"
from camelcase import CamelCase

c = CamelCase()
print(c.hump('hello there world'))
```
This'll make the first charcter of each word uppercase
> *Hello There World*
