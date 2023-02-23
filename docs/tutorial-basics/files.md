---
sidebar_position: 12
---

# Working with Files
Python has functions for creating, reading, updating, and deleting files.

## Open a file
To open a file, use the `open()` function. Pass in the filename and specify the mode (w stands for 'write', so we want to write to the file):If the file already exists, then i'll opened. If not, then a new file is created at that location.

```
myFile = open('myfile.txt', 'w')
```
If you run the file, a new file named my.file.txt will be created in the current directory of your computer.

## Get the file info
You can get information about the file:
```
print('Name: ', myFile.name)
print('Is Closed : ', myFile.closed)
print('Opening Mode: ', myFile.mode)
```
Here we're getting the file name, mode and if the file is open or closed. If you run the code, you'll get the follwoing output:

> Name: myfile.txt

> Is Closed: False

> Opening Mode: w

## Write to the file
To add text to the file, use the write() method:
```
myFile.write('I love Python')
myFile.write(' and JavaScript')
myFile.close()
```
This writes the text "I love Python and JavaScript" to the file and closes it.

## Append to a file
You can append text to a file with the append() method:
```
myFile = open('myfile.txt', 'a')
myFile.write(' I also like PHP')
myFile.close()
```
First you need to open the file (since it was closed).

## Read from a file
To read from a file, you need to use r+ mode in the second argument of open():

```
# Read from file
myFile = open('myfile.txt', 'r+')
text = myFile.read(100)
print(text)
```
Here we're reading 100 chracters from the file. If you run the code, you'll get the following output:
> *I love Python and JavaScript I also like PHP*