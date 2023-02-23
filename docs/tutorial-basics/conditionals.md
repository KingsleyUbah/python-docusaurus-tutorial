---
sidebar_position: 8
---

# Conditionals
Comparison and Logical operators are used to test for true or false.

- If/ Else conditions are used to decide to do something based on something being true or false
- Comparison Operators (==, !=, >, <, >=, <=) - Used to compare values
- Membership Operators (not, not in) - used to test if a sequence is presented in an object

## Simple `if` statement
The following if statement prints the provided text if x is greater than y:
```python title="my-python-app/conditionals.py"
x = 21
y = 20

if x > y:
    print(f'{x} is greater than {y}')
```
If you ran the code, you'll get the following output:
> 21 is greater than 20

## If/else
If you want to execute something if the condition is not trye, nest an else block to `if`:
```python title="my-python-app/conditionals.py"
x = 10
y = 59

if x > y:
    print(f'{x} is greater than {y}')
else: 
    print(f'{y} is greater than {x}')
```
In this case, the else block will run because the if block is not true.

## elif
You can create multiple in-between brances to run code when the right trigger is activated. This is done using `elif`.
```python title="my-python-app/conditionals.py"
# elif
if x > y:
  print(f'{x} is greater than {y}')
elif x == y:
  print(f'{x} is equal to {y}')  
else:
  print(f'{y} is greater than {x}')  
```
S in this case, we add a third branch to account for siutations where x and y are equal.

## Logical Operators
```python title="my-python-app/conditionals.py"
# and
if x > 2 and x <= 10:
    print(f'{x} is greater than 2 and less than or equal to 10')
```

```python title="my-python-app/conditionals.py"
# or
if x > 2 or x <= 10:
    print(f'{x} is greater than 2 or less than or equal to 10')
```

```python title="my-python-app/conditionals.py"
# not
if not(x == y):
  print(f'{x} is not equal to {y}')
```

# Membership operator

```python title="my-python-app/conditionals.py"
numbers = [1,2,3,4,5]

#  in
if x in numbers:
  print(x in numbers)

# not in
if x not in numbers:
  print(x not in numbers)
```