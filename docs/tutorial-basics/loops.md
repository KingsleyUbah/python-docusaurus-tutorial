# Loops
A for loop is used for iterating over a sequence (that is either a list, a tuple, a dictionary, a set, or a string).

## Simple for loop
Here's a simple for loop that cycles through people list and prints the current person on each iteration:
```python title="my-python-app/loops.py"
people = ['John', 'Paul', 'Sara', 'Susan']

for person in people:
  print(f'Current Person: {person}')
```
If you run the above code, you'll get the following output:

> *Current Person: John*

> *Current Person: Paul*

> *Current Person: Sarah*

> *Current Person: Susan*

## Break
You can also break out of a loop when a specific condition is met.

In this example, we break the loop once it gets to Sarah, so the remaning items will not be iterated over"
```python title="my-python-app/loops.py"
for person in people:
  if person == 'Sara':
    break
  print(f'Current Person: {person}')
```
This'll be the output:
> *Current Person: John*

> *Current Person: Paul*

## Continue
The continue statement is used to skip an iteration when a specific condition is mey.

In this example, we skip the loop once it gets to Sarah:
```python title="my-python-app/loops.py"
for person in people:
  if person == 'Sara':
    continue
  print(f'Current Person: {person}')
```
If you run the code, this'll be the output:
> *Current Person: John*

> *Current Person: Paul*

> *Current Person: Sarah*

> *Current Person: Susan*

## range
```python title="my-python-app/loops.py"
for i in range(len(people)):
  print(people[i])

for i in range(0, 11):
  print(f'Number: {i}')
```

## while

```python title="my-python-app/loops.py"
count = 0
while count < 10:
  print(f'Count: {count}')
  count += 1
```



