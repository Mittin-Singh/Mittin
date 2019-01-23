---
layout: post
title: 'Python Introduction '
date: {}
excerpt: A ton of text to test readability.
tags:
  - sample post
  - readability
  - test
comments: true
published: false
---

![](../imgs/python_logo.png)
<br>

In this tutorial, we will introduce you to Python Programming. We will discuss about features of Python, Python architecture and its applications in the IT industry. Also, we will learn about Python in Data Science|Big Data|Machine Learning etc. and we will also prepare for Interview Questionaires as well.

There’s a reason they choose Python as an introductory language for programming. 
Simplicity 
Concise
Easiness to grasp Python Concept. 

It also equips you to build so much.

#                               So, let’s start this Python Tutorial.

## 1. What is Python ?

Python is a widely used general-purpose, high level, Orthogonal programming language. It is also dynamically-typed because it carries out type-checking at runtime. It was initially designed by Guido van Rossum in 1991 and developed by Python Software Foundation. It was mainly developed for emphasis on code readability, and its syntax allows programmers to express concepts in fewer lines of code.The Python IDLE (Integrated Development Environment) executes instructions one line at a time. This also lets us use it as a calculator.

Python is a programming language that lets you work quickly and integrate systems more efficiently.

## 2. Why it is called Python ?

Guido van Rossum named it after the comedy group Monty Python. A lot of implementations today run version 2.x, but the future belongs to Python 3.x. It is also called ‘Python 3000’ or ‘Py3K’. CPython, written in C, is the most common implementation of Python.

## 3. Origin of Python ?

The Python programming language was conceived in the late 1980s and was named after the BBC TV show Monty Python’s Flying Circus. Guido van Rossum started implementing Python at CWI (Centrum Wiskunde & Informatica) in the Netherlands in December of 1989. This was a successor to the ABC programming language which was capable of exception handling and interfacing with the Amoeba operating system.

On October 16 of 2000, Python 2.0 released and it had many major new features including cycle-detecting garbage collector for memory management and support for Unicode.

The next version of Python 3.0 released on December 3, 2008.

## 4. Architechture of Python ?

Let’s now talk about Python architecture and its usual flow –

-Parser

It uses the source code to generate an abstract syntax tree.

-Compiler

It turns the abstract syntax tree into Python bytecode.

-Interpreter

It executes the code line by line in a REPL (Read-Evaluate-Print-Loop) fashion. 

## 5. Python Constructs ?

i. Functions
A function in Python is a collection of statements grouped under a name. You can use it whenever you want to execute all those statements at a time. You can call it wherever you want and as many times as you want in a program. A function may return a value.

ii. Classes
As we discussed earlier, Python is an object-oriented language. It supports classes and objects. A class is an abstract data type. In other words, it is a blueprint for an object of a certain kind. It holds no values. An object is a real-world entity and an instance of a class.

iii. Modules
A Python module is a collection of related classes and functions. We have modules for mathematical calculations, string manipulations, web programming, and many more. We will discuss Python Module in detail in a later lesson.

iv. Packages
Python package is a collection of related modules. You can either import a package or create your own.

v. List
You can think of a list as a collection of values. Declared in the CSV (Comma-Separated Values) format and delimit using square brackets:

life = [‘love’, ‘wisdom’, ‘anxiety’];
arity = [1,2,3];
Notice that we do not declare the type for the list either. A list may also contain elements of different types, and the indexing begins at 0:

person = [‘firstname’, 21];
print(person[1])
Output: 21
You can also slice lists; slicing is a way of retrieving some values from it. We will learn more about it in further lessons.

vi. Tuple
A tuple is like a list, but it is immutable (you cannot change its values).

pizza = (‘base’, ‘sauce’, ‘cheese’, ‘mushroom’);
pizza[3] = ‘jalapeno’
This raises a TypeError.

vii. Dictionary
A dictionary is a collection of key-value pairs. Declare it using curly braces, and commas to separate key-value pairs. Also, separate values from keys using a colon (:).

student = {‘Name’: ‘Abc’, ‘Age’: 21}
print(student[‘Age’])
Output: 21

viii. Comments and Docstrings
Declare comments using an octothorpe (#). However, Python does not support multiline comments. Also, docstrings are documentation strings that help explain the code.

#This is a comment
“““
This is a docstring
”””
Python has a lot of other constructs. These include control structures, functions, exceptions, etc. We will discuss these in further tutorials.

## 5. Python Features

i. Easy

Python is very easy to learn and understand; using this Python tutorial, any beginner can understand the basics of Python.

ii. Interpreted

It is interpreted(executed) line by line. This makes it easy to test and debug.

iii. Object-Oriented

The Python programming language supports classes and objects. We discussed these above.

iv. Free and Open Source

The language and its source code are available to the public for free; there is no need to buy a costly license.

v. Portable

Since it is open-source, you can run Python on Windows, Mac, Linux or any other platform. Your programs will work without needing to the changed for every machine.

vi. GUI Programming

You can use it to develop a GUI (Graphical User Interface). One way to do this is through Tkinter.

vii. Large Library

Python provides you with a large standard library. You can use it to implement a variety of functions without needing to reinvent the wheel every time. Just pick the code you need and continue. This lets you focus on other important tasks.

## 6. Flavors of Python

i. CPython
This is the most widely accepted implementation of Python. It is written in the language C, and is an interpreter.

ii. Jython
Jython is a Python implementation written in Java. A Jython program can import any Java class. It compiles to Java bytecode.

iii. IronPython
IronPython is implemented in C#. It can function as an extensibility layer to application frameworks written in a .NET language.

iv. Brython
Brython stands for Browser Python. It is an implementation of Python that runs in the browser.

v. RubyPython
It acts as a bridge between the Python and Ruby interpreters. It marshals data between Python and Ruby virtual machines.

vi. PyPy
Interesting to know how PyPy is Python implemented in Python. This makes it faster and easier to experiment with. However, the standard implementation is CPython.

vii. MicroPython
This is an implementation of Python meant to run on a microcontroller. It uses a MicroPython board that runs MicroPython on bare metal.

## 7. File Extensions in Python

- py –The normal extension for a Python source file
- pyc- The compiled bytecode
- pyd- A Windows DLL file
- pyo- A file created with optimizations
- pyw- A Python script for Windows
- pyz- A Python script archive


# Thanks !!!

## Furthermore, if you have any query, feel free to ask in the comment section.