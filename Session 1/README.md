# Details of Python Basics Session 1
## In this document it is mentioned that all the points that are discussed in the Python Class Session 1.

### Introduction
#### About Python
Python is a widely used general-purpose, high level programming language. It was created by Guido van Rossum in 1991 and further developed by the Python Software Foundation. It was designed with an emphasis on code readability, and its syntax allows programmers to express their concepts in fewer lines of code.

#### What can Python do?
- Python can be used on a server to create web applications.
- Python can be used alongside software to create workflows.
- Python can connect to database systems. It can also read and modify files.
- Python can be used to handle big data and perform complex mathematics.
- Python can be used for rapid prototyping, or for production-ready software development.

#### Why Python?
- Python works on different platforms (Windows, Mac, Linux, Raspberry Pi, etc).
- Python has a simple syntax similar to the English language.
- Python has syntax that allows developers to write programs with fewer lines than some other programming languages.
- Python runs on an interpreter system, meaning that code can be executed as soon as it is written. This means that prototyping can be very quick.
- Python can be treated in a procedural way, an object-oriented way or a functional way.

#### Difference between Python 2 and Python 3
![Differences](../python_difference.png)

### Installation
#### Installing Python
- Visit https://python.org and download python and also make sure to install it for all users in your system.
#### Installing VS Code**
- Visit https://code.visualstudio.com and download VS Code and then install it in your system. 
- Download Python Extension from the extension tab at the let side of VS code or you can also install the plugin bu visiting [here.](https://marketplace.visualstudio.com/items?itemName=ms-python.python)

### Language Overview
#### Hello World Program and Zen of Python
- [Hello World Program](Chap01/hello.py)
- Zen of Python
    ```
    >> import this
    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!
    ```


#### Variables, Expression and Statements
**Variables**: It is a place where we can store values. Instead of using the values directly, we can refer the variable name where the actual values are stored.
```
> x = 2 === > here X is Variable
> name = 'John' === > here NAME is variable
```
**Expression**: It contains values, variables and operators.
```
> 10
> x
> y = x + 10
```
**Statements**:It is a logical unit of code that can be executed at the Python interpreter. When we type statement at the command promt, it will execute the code in the statement then provides the results, as long as the code is clean. We can execute code that is in a file. In general these file contains scripts, these scripts are combination of statements to perform units of work. (Every line of code ioa called statement)
```
> print("Hello World")
Hello World
```

#### Indentation and Comments
**Python Indentation**: Most of the programming languages like C, C++, and Java use braces { } to define a block of code. Python, however, uses indentation. A code block (body of a function, loop, etc.) starts with indentation and ends with the first unindented line. The amount of indentation is up to you, but it must be consistent throughout that block.

Generally, four whitespaces are used for indentation and are preferred over tabs. Here is an example.

```
for i in range(1,11):
    print(i)
    if i == 5:
        break
```

The enforcement of indentation in Python makes the code look neat and clean. This results in Python programs that look similar and consistent.
Indentation can be ignored in line continuation, but it's always a good idea to indent. It makes the code more readable. For example:

```
if True:
    print('Hello')
    a = 5
```
and
```
if True: print('Hello'); a = 5
```
both are valid and do the same thing, but the former style is clearer.
Incorrect indentation will result in ```IndentationError```.

**Python Comments**: Comments are very important while writing a program. They describe what is going on inside a program, so that a person looking at the source code does not have a hard time figuring it out. You might forget the key details of the program you just wrote in a month's time. So taking the time to explain these concepts in the form of comments is always fruitful.

In Python, we use the hash (#) symbol to start writing a comment.
It extends up to the newline character. Comments are for programmers to better understand a program. Python Interpreter ignores comments.
```
# This is a comment
# print out Hello
print('Hello')
```
Another way of doing this is to use triple quotes, either ```'''``` or ```"""```.
These triple quotes are generally used for multi-line strings. But they can be used as a multi-line comment as well. Unless they are not docstrings, they do not generate any extra code.
```
"""This is also a
perfect example of
multi-line comments"""
```

#### Using print()
The simplest way to produce output is using the print() function where you can pass zero or more expressions separated by commas. This function converts the expressions you pass into a string before writing to the screen.
There are 2 common ways to print output, One, using format and Second, Cohersion/concatination. However, concatination only supports the same satatypes to be included but format supports all data types. 
```
#!/usr/bin/env python3
# Copyright 2009-2017 BHG http://bw.org/

import platform

# Using format
print('This is python version {}'.format(platform.python_version()))
# Using concatination by converting the version of python whcih is in number to string using str function. 
print('This is python version ' + str(platform.python_version()))
```

#### Blocks
A block is a group of statements in a program or script. Usually, it consists of at least one statement and declarations for the block, depending on the programming or scripting language. A language which allows grouping with blocks, is called a block structured language. Generally, blocks can contain blocks as well, so we get a nested block structure. A block in a script or program functions as a means to group statements to be treated as if they were one statement. In many cases, it also serves as a way to limit the lexical scope of variables and functions.
Python uses a different principle. Python programs get structured through indentation, i.e. code blocks are defined by their indentation. Okay that's what we expect from any program code, isn't it? Yes, but in the case of Python it's a language requirement, not a matter of style. This principle makes it easier to read and understand other people's Python code.

![Block Structure](https://www.python-course.eu/images/blocks.png)

```
from math import sqrt
n = input("Maximum Number? ")
n = int(n)+1
for a in range(1,n):
    for b in range(a,n):
        c_square = a**2 + b**2
        c = int(sqrt(c_square))
        if ((c_square - c**2) == 0):
            print(a, b, c)
```

#### Contitionals
![If-else conditional flowchart](http://1.bp.blogspot.com/-3aE4DKXIGf0/UQ3q4RPUSSI/AAAAAAAAA2I/0NsrJ2hnLr0/s1600/if-else.jpg)

Conditional statements that controls execution of the program with conditions by validating expressions that we provide. As we saw in the above example it uses if or else condition the execute and validate the code execution. To see the program visit this [link](Chap02/blocks.py)

In Python, there are mainly 3 conditional statements or you can call them as keywords as well, ```if```, ```elif``` and ```else```. To understand this in a simple way, when program is running it checks the ```if``` condition block first and then later on if ```elif``` block exists, it checks that condition too (if ```if``` block condition is false) and finally it checks ```else``` block for whatever the remaining condition.

It is not mandatory to have all 3 conditions in the code, progrma work even for only ```if``` condition existance. You can refer to the above program for the example. 

#### Loops
![Flow](https://www.tutorialspoint.com/python/images/loop_architecture.jpg)

There are mainly 3 loops are there in Python,
1. ```for``` loops 
    - [Example](Chap02/for.py)
2. ```while``` loops
    - [Example](Chap02/while.py)
3. Nested loops
    - [Example](Chap02/nested.py)

### References:
1. [About Python](https://www.geeksforgeeks.org/python-language-introduction/#:~:text=Python%20is%20a%20widely%20used,in%20fewer%20lines%20of%20code.)
2. [Why Python?](https://www.w3schools.com/python/python_intro.asp)
3. [Python 2 and 3 Difference](https://www.differencebetween.com/difference-between-python-2-and-vs-3/)
4. [Variables, Expression and Statements](https://www.wisdomaxis.com/technology/software/python/what-is-Python-Variable-Expression-Statement.php)
5. [Indentation and Comments](https://www.programiz.com/python-programming/statement-indentation-comments)
6. [Python Blocks](https://www.python-course.eu/python3_blocks.php)

### Missed Topics
1. Scope
2. Control Statements
3. Nested Loops (do...while)
4. Functions
5. Objects

