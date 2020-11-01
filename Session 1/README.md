# Details of Python Basics Session 1
## In this document it is mentioned that all the points that are discussed in the Python Class Session 1.

### Topics Discussed
- Author of Python
- Zen of Python by Tim Peters
- Difference Between Python 2 and Python 3
- Installation of Python
- Installation of PyCharm
- Checking the Status of Python Installation in CLI
- Overview of IDE
- Difference Between IDE and Code Editor
- Running "Hello, World!" Program
- Python Comments
- Hash Bang (Shabang) Comments
- **import** keyword and **modules/libraries** 
- Statements
- Print Function in Python 2 and Python 3

#### Introduction
**About Python**
Python is a widely used general-purpose, high level programming language. It was created by Guido van Rossum in 1991 and further developed by the Python Software Foundation. It was designed with an emphasis on code readability, and its syntax allows programmers to express their concepts in fewer lines of code.

**What can Python do?**
- Python can be used on a server to create web applications.
- Python can be used alongside software to create workflows.
- Python can connect to database systems. It can also read and modify files.
- Python can be used to handle big data and perform complex mathematics.
- Python can be used for rapid prototyping, or for production-ready software development.

**Why Python?**
- Python works on different platforms (Windows, Mac, Linux, Raspberry Pi, etc).
- Python has a simple syntax similar to the English language.
- Python has syntax that allows developers to write programs with fewer lines than some other programming languages.
- Python runs on an interpreter system, meaning that code can be executed as soon as it is written. This means that prototyping can be very quick.
- Python can be treated in a procedural way, an object-oriented way or a functional way.

**Difference between Python 2 and Python 3**
![Differences](python_difference.png)

#### Installation
**Installing Python**
- Visit https://python.org and download python and also make sure to install it for all users in your system.
**Installing VS Code**
- Visit https://code.visualstudio.com and download VS Code and then install it in your system. 
- Download Python Extension from the extension tab at the let side of VS code or you can also install the plugin bu visiting [here.](https://marketplace.visualstudio.com/items?itemName=ms-python.python)

#### Language Overview
- [Hello World Program](Chap01/hello.py)

**Variables, Expression and Statements**
_Variables_: It is a place where we can store values. Instead of using the values directly, we can refer the variable name where the actual values are stored.
```
> x = 2 === > here X is Variable
> name = 'John' === > here NAME is variable
```
_Expression_: It contains values, variables and operators.
```
> 10
> x
> y = x + 10
```
_Statements_:It is a logical unit of code that can be executed at the Python interpreter. When we type statement at the command promt, it will execute the code in the statement then provides the results, as long as the code is clean. We can execute code that is in a file. In general these file contains scripts, these scripts are combination of statements to perform units of work. (Every line of code ioa called statement)
```
> print("Hello World")
Hello World
```

**Indentation and Comments**
_Python Indentation_: Most of the programming languages like C, C++, and Java use braces { } to define a block of code. Python, however, uses indentation. A code block (body of a function, loop, etc.) starts with indentation and ends with the first unindented line. The amount of indentation is up to you, but it must be consistent throughout that block.

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
- Using print()
- Blocks and Scope
- Contitionals
- Loops
- Functions
- Objects


References:
1. [About Python](https://www.geeksforgeeks.org/python-language-introduction/#:~:text=Python%20is%20a%20widely%20used,in%20fewer%20lines%20of%20code.)
2. [Why Python?](https://www.w3schools.com/python/python_intro.asp)
3. [Python 2 and 3 Difference](https://www.differencebetween.com/difference-between-python-2-and-vs-3/)
4. [Variables, Expression and Statements](https://www.wisdomaxis.com/technology/software/python/what-is-Python-Variable-Expression-Statement.php)

