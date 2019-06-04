---
layout: post
title: 'Python Structuring with Indentation'
date: 2019-01-26
excerpt: Intendation in Python Language.
tags:
  - Python
  - Programming
comments: true
published: true
---
# Python Structuring with Indentation

![](../img/pythonlogo.jpg)
<br>

A block is a group of statements in a program or script. Usually it consists of at least one statement and of declarations for the block, depending on the programming or scripting language. A language, which allows grouping with blocks, is called a block structured language. Generally, blocks can contain blocks as well, so we get a nested block structure. A block in a script or program functions as a mean to group statements to be treated as if they were one statement. In many cases, it also serves as a way to limit the lexical scope of variables and functions.

Initially, in simple languages like Basic and Fortran, there was no way of explicitly using block structures. Programmers had to rely on "go to" structures, nowadays frowned upon, because "Go to programs" turn easily into spaghetti code, i.e. tangled and inscrutable control structures.

The first time, block structures had been formalized was in ALGOL, called a compound statement.

Programming languages usually use certain methods to group statements into blocks:
- begin ... end<br>
  ALGOL, Pascal and others<br>
  An code snippet in Pascal to show this usage of blocks:

            with ptoNode^ do
            begin
                x := 42;
                y := 'X';
            end;

- do ... done
e.g. Bourne and Bash shell
- Braces (also called curly brackets): { ... }<br>
By far the most common approach, used by C, C++, Perl, Java, and many other programming languages are braces.<br>
The following examples shows a conditional statement in C:
        if (x==42) {
            printf("The Answer to the Ultimate Question of Life, the Universe, and Everything\n");
        } else {
            printf("Just a number!\n");
        }
The indentations in this code fragment are not necessary. So the code could be written - offending common decency - as
      if (x==42) {printf("The  Answer to the Ultimate Question of Life, the Universe, and Everything\n");} else {printf("Just a number!\n");}
Please, keep this in mind to understand the advantages of Python!
- if ... fi
e.g. Bourne and Bash shell

## Indenting Code

Python uses a different principle. Python programs get structured through indentation, i.e. code blocks are defined by their indentation. Okay that's what we expect from any program code, isn't it? Yes, but in the case of Python it's a language requirement not a matter of style. This principle makes it easier to read and understand other people's Python code.

So, how does it work? All statements with the same distance to the right belong to the same block of code, i.e. the statements within a block line up vertically. The block ends at a line less indented or the end of the file. If a block has to be more deeply nested, it is simply indented further to the right.

Beginners are not supposed to understand the following example, because we haven't introduced most of the used structures, like conditional statements and loops. Please confer the following chapters about loops and conditional statements for explanations.
The program implements an algorithm to calculate Pythagorean triples. You will find an explanation of the Pythagorean numbers in our chapter on for loops.

    from math import sqrt
    n = input("Maximum Number? ")
    n = int(n)+1
    for a in range(1,n):
        for b in range(a,n):
            c_square = a**2 + b**2
            c = int(sqrt(c_square))
            if ((c_square - c**2) == 0):
                print(a, b, c)

There is another aspect of structuring in Python, which we haven't mentioned so far, which you can see in the example. Loops and Conditional statements end with a colon ":" - the same is true for functions and other structures introducing blocks. So, we should have said Python structures by colons and indentation.

## Zen of Python

- Beautiful is better than ugly.
- Explicit is better than implicit.
- Simple is better than complex.
- Complex is better than complicated.
- Flat is better than nested.
- Sparse is better than dense.
- Readability counts.
- Special cases aren't special enough to break the rules.
- Although practicality beats purity.
- Errors should never pass silently.
- Unless explicitly silenced.
- In the face of ambiguity, refuse the temptation to guess.
- There should be one -- and preferably only one -- obvious way to do it.
- Although that way may not be obvious at first unless you're Dutch.
- Now is better than never.
- Although never is often better than *right* now.
- If the implementation is hard to explain, it's a bad idea.
- If the implementation is easy to explain, it may be a good idea.
- Namespaces are one honking great idea -- let's do more of those!

## Development Steps towards Python

Guido Van Rossum published the first version of Python code (version 0.9.0) at alt.sources in February 1991. This release included already exception handling, functions, and the core data types of list, dict, str and others. It was also object oriented and had a module system.

Python version 1.0 was released in January 1994. The major new features included in this release were the functional programming tools lambda, map, filter and reduce, which Guido Van Rossum never liked.

Six and a half years later in October 2000, Python 2.0 was introduced. This release included list comprehensions, a full garbage collector and it was supporting Unicode.

Python flourished for another 8 years in the versions 2.x before the next major release as Python 3.0 (also known as "Python 3000" and "Py3K") was released. Python 3 is not backwards compatible with Python 2.x. The emphasis in Python 3 had been on the removal of duplicate programming constructs and modules, thus fulfilling or coming close to fulfilling the 13th law of the Zen of Python: "There should be one -- and preferably only one -- obvious way to do it."

### Some changes in Python 3.0:

- Print is now a function
- Views and iterators instead of lists
- The rules for ordering comparisons have been simplified. E.g. a heterogeneous list cannot be sorted, because all the elements of a list must be comparable to each other.
- There is only one integer type left, i.e. int. long is int as well.
- The division of two integers returns a float instead of an integer. "//" can be used to have the "old" behaviour.
- Text Vs. Data Instead Of Unicode Vs. 8-bit

# Thanks !!!

## Furthermore, if you have any query, feel free to ask in the comment section.
