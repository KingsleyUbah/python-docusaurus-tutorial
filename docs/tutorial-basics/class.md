---
sidebar_position: 11
---

# Classes
A class is like a blueprint for creating objects. An object has properties and methods(functions) associated with it. Almost everything in Python is an object.

### Create a class
To create a class, use the `Class` keyword:

```python title="my-python-app/class.py"
# Create class
class User:

  # Constructor
  def __init__(self, name, email, age):
    self.name = name
    self.email = email
    self.age = age
    self._private = 1000 

  def greeting(self):
      return f'My name is {self.name} and I am {self.age}'

  def has_birthday(self):
      self.age += 1
 
 #function for encap variable
  def print_encap(self):
      print(self._private)
```
This `User` class has four properties namely name, email, age and a private field. It also has methods:
- gretting(): Says the name
- has_birthday: Increments the age by 1
- print_encap(): Prints the private variable

Now let's initialize an object from the User class:
```python title="my-python-app/class.py"
#  Init user object
brad = User('Brad Traversy', 'brad@gmail.com', 37)
print(brad.greeting())
```
We pass the name, email and age, which are all required by the constructor on initialization. If you rin the above code, you'll get the output of thr greeting method:

> *My name is brad and I am 37* 

