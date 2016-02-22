# Programming Basics

It's always worthwhile to keep in mind why we are doing something, particularly when we are trying to learn a new skill such as a programming language. If we don't, then we can very quickly get overwhelmed by the enormous

By the end of our two bootcamp sessions, we'd like to be able to do the following in Python: 
* Input some data, presumably from a file
* Manipulate this data until it's in the form we want
* Perform some simple analyses
* Produce a compelling graphic

Those are the goals for the bootcamp. For today, though, we're going to start with the much less ambitious goal of making sure that that we're all on the same page in terms of basic Python. 
Specifically, for today we'll be covering the following:

* Jupyter Notebook
* Python Basics
	- Fundamental data types, such as numbers, strings, lists, etc
	- Calculations using fundamental data types
	- Controlling the flow in a Python program

**Jupyter Notebook Basics**

* Entering and executing Python
* Documenting what you've done

**Python Basics Pt 1**

* Numbers and Calculations
* Comments
* Assignments
* Built-in functions (print, type), 
* Strings and Quotes
* Flow of Control

**Python Basics Pt 2**

* Lists
* Extending Python by Importing Packages
* Objects and Methods
* Tab Completion
* Getting help

# Numbers and Calculations

Python has various "types" of numbers (numeric literals). We'll mainly focus on integers and floating point numbers.

* Integers are just whole numbers, positive or negative. For example: 2 and -2 are examples of integers.

* Floating point numbers in Python are notable because they have a decimal point in them, or use an exponential (e) to define the number. For example 2.0 and -2.1 are examples of floating point numbers. 4E2 (4 times 10 to the power of 2) is also an example of a floating point number in Python.

The most basic functionality that I can imagine for using Python is to use an interactive shell as a calculator. 
As a starting point, let's take a few minutes to run through the most basic arithmetic operations. 
In each of the cells below, enter an expression that will return the requested results. 
Remember, after you type the expression, hit <CTL>-return to execute the cell.

To get you started, here are some of the most fundamental arithmetic operations:

| Operator | Function |
|:--------:|:--------:|
| + | Addition |
| - | Subtraction | 
| * | Multiplication |
| / | Division |

<div class="alert alert-info" role="alert">
You may have noticed that each of the cells in this notebook starts with a line that begins with a hashtag or "#". This hashtag tells Python that the line should be considered as a comment and shouldn't be executed. 
</div>

```python
>>> # add two integers, say 1 and 2
>>>
>>> None
```

```python
>>> # multiply 2 integers, say 2 and 3
>>> 
>>> None
```

```python
>>> # now divide 2 integers, say 3 by 2 as
>>> # 3 / 2
>>> # pay attention to what happens here
>>>
>>> None
```

```python
>>> # In Python 2, when we divide two integers, we get what's called "classic" division within the Python community.
>>> # We can avoid this "classic" division, by making sure that one of the numbers is a floating point number, for example try
>>> # 3.0 / 2
>>> 
>>> None
```

```python
>>> # And, in this case, the order in which we use the floating point number doesn't matter.
>>> # 3 / 2.0
>>> 
>>> None
```

```python
>>> # We can force the issue by using the "float()" function to "cast" one of the integers to be a floating point number.
>>> # Note: we'll talk more about functions in a little while, but for now
>>> # float(3) / 2
>>>
>>> None
```

```python
>>> # Finally, we can control the order in which operations are executed using parentheses, for instance, try
>>> # 2 * 3 + 4
>>>
>>> None
```

```python
>>> # and conversely, notice the difference is we use the following
>>> # 2 * ( 3 + 4 )
>>>
>>> None
```

So what happened here? By default, Python has a specific order in which it will execute operations. As a rule, it will perform multiplication before addition. 
In these final examples, the parentheses are introduced to force the expression "3 + 4" to be executed first.
If you are completely new to programming, this can be a bit confusing and I recommend that you take a look at the Python documentation for more detail on the order in which operations are executed.

# Assigning Variables

If we could only use Python as a calculator to evaluate expressions, then we'd be pretty limited in terms of the types of problems that we could solve. As a first step in moving towards more interesting computations, We can store results by assigning a label, or a variable name, to our results as we move along. For example, let's say that we want to store the value "10" using a variable named "a".

Python does this as:

```python
>>>  a = 10
```

Try it in the cell below:

```python
>>> None
```

If you typed that in exactly as shown, then you shouldn't have gotten any type of output. There are a couple of ways in which we can test whether or not, the variable was actually set though.

First, you can simply evaluate a cell with the name of the variable:

```python
>>> a
10
```

Alternatively, you can use the "print" function in python which will evaluate an expression (in this case the variable) and print the results to the screen. In Python 2, the syntax for this is:

```python
>>> print a
10
```

In terms of creating variable names, there are some rules on what's allowable:

1. Names can not start with a number.
2. There can be no spaces in the name
3. Can't use any of these symbols :,'<>"/?|\()!@#$%^&*~-+

Using variable names can be a very useful way to keep track of different variables in Python. For example:

1. It's considered best practice that the names are lowercase.
2. Also, if you need to create a long name, maybe comprised of several words string together, Python best practice is to connect these words using underscores. e.g. this_is_johns_variable

## Review

Construct a series of expressions to compute the taxes you would need to pay on a typical data scientists sallary. 
Assume the following:

* My income is $ 20,000,000
* My tax rate is 30%

As a simple exercise, please set up variables called my_income and my_tax_rate compute the taxes you owe using simnple multiplication. Finally, print out the taxes you owe.

```python
>>> # Build your simple computation here
>>>
>>> None
```

## Answer

Your answer should look something like the following

```python
>>> my_income = 20000000
>>> my_tax_rate = 0.30
>>> my_taxes = my_income * my_tax_rate
>>> print my_taxes
6000000.0
```

When you evaluate your results, you should get something like:

```
 Out [ ]: 6000000.0
```

    
Depending on how you actually entered the lines of code, you may not have gotten the "Out" prompt

# Other Fundamental Data Types in Python

## Objects in Python

## Strings

* Double quotes or single quotes
* Index from 0
* Slicing
* Does not include the right index "up to but not including"
* Include everything
* Negative indexing
* frequency / step size / reversing a sting using a -1 step size

### String Properties

Strings are immutable, i.e. once they are created, they can't be changed or replaced.
Concatenation using + 
Duplication using *

### String Methods

Actions on the objects themselves

```python
>>> len('Hello world!')
12
```

```python
>>> s = 'Hello world'
>>> print s[::-1]
dlrow olleH
```

```python
>>> s + ' there'
'Hello world there'
```

```python
>>> s*2
'Hello worldHello world'
```

```python
>>> s = 'hello'
>>> s.upper()
'HELLO'
```

```python
>>> s.capitalize()
'Hello'
```

```python
>>> s.find('l')
2
```

```python
>>> s.split('e')
['h', 'llo']
```

## Lists

Enter descriptive text here

```python
>>> my_list = [1,2,3]
>>> print my_list
[1, 2, 3]
```

```python
>>> my_list = ['string', 23, 1.234, '0']
>>> len(my_list)
4
```

### Index and Slicing

* Works just like strings
* can do list concatenation

* no fixed sizes in list
* no type constraints on contents

### List Methods

```python
>>> l = [1,2,3]
>>> l.append('append me')
>>> print l
[1, 2, 3, 'append me']
```

```python
>>> l.pop()
'append me'
```

```python
>>> l = [1, 2, 3]
>>> l.pop(0)
1
```

```python
>>> print l
[2, 3]
```

```python
>>> new_list = ['a', 'e', 'x', 'b', 'c']
>>> print new_list
['a', 'e', 'x', 'b', 'c']
```

```python
>>> new_list.reverse()
>>> print new_list
['c', 'b', 'x', 'e', 'a']
```

```python
>>> new_list.sort()
>>> print new_list
['a', 'b', 'c', 'e', 'x']
```

### List Comprehensions

Enter descriptive text here

```python
>>> l_1 = [1,2,3]
>>> l_2 = [4,5,6]
>>> l_3 = [7,8,9]
>>> matrix = [l_1, l_2, l_3]
>>> first_column = [row[0] for row in matrix]
>>> print first_column
[1, 4, 7]
```

## Matrices

In python, we can create a data structure called a **matrix** which is a nested collection of lists. For instance:

```python
>>> l_1 = [1,2,3]
>>> l_2 = [4,5,6]
>>> l_3 = [7,8,9]
>>> matrix = [l_1, l_2, l_3]
>>> print matrix
```

```python
>>> print matrix[0]
[1, 2, 3]
```

```python
>>> print matrix[1][2]
6
```

## Dictionaries

A dictionary is basically a mapping between objects. What we've seen so far are sequences, objects where we can index them based on their position. keys must be unique

```python
>>> my_dict = {'key1': 'value', 'key2': 'value2'}
>>> print my_dict
{'key2': 'value2', 'key1': 'value'}
```

```python
>>> my_dict['key1']
'value'
```

```python
>>> my_dict = {'key1': 'value', 'key2': 123, 'key3': [1,2,3]}
```

```python
>>> my_dict['key1']
'value'
```

```python
>>> my_dict['key3']
[1, 2, 3]
```

```python
>>> my_dict['key3'].pop()
3
```

```python
>>> my_dict
{'key1': 'value', 'key2': 123, 'key3': [1, 2]}
```

```python
>>> my_dict['key1'].upper()
'VALUE'
```

```python
>>> my_dict
{'key1': 'value', 'key2': 123, 'key3': [1, 2]}
```

```python
>>> my_dict['key2'] *= 2
```

```python
>>>  my_dict
{'key1': 'value', 'key2': 246, 'key3': [1, 2]}
```

```python
>>> d = {}
>>> d
{}
```

```python
>>> d['animal'] = 'Dog'
>>> d['answer'] = 42
```

```python
>>> d
{'animal': 'Dog', 'answer': 42}
```

```python
>>> d = {'k1': {'nestKey': {'subnest': 'value'}}}
>>> print d
{'k1': {'nestKey': {'subnest': 'value'}}}
```

```python
>>> d['k1']
{'nestKey': {'subnest': 'value'}}
```

```python
>>> d['k1']['nestKey']['subnest'].upper()
'VALUE'
```

```python
>>> d = {}
```

```python
>>> d['k1'] = 1
>>> d['k2'] = 2
>>> d['k3'] = 3
>>> print d
{'k3': 3, 'k2': 2, 'k1': 1}
```

```python
>>> d.keys()       # note the order. Dictionaries do not guarantee any order
['k3', 'k2', 'k1']
```

```python
>>> d.values()
[3, 2, 1]
```

```python
>>> d.items()       # this returns tuples of all of the dictionary key-value pairs
[('k3', 3), ('k2', 2), ('k1', 1)]
```

## Tuples

Similar to lists but immutable

```python
>>> t = (1,2,3)
>>> print t
(1, 2, 3)
```

```python
>>> len(t)
3
```

```python
>>> t[1]
2
```

```python
>>> t = ('one', 2)
```

```python
>>> print t[0]
one
```

```python
>>> print t[1]
2
```

```python
>>> print t[-1]
2
```

```python
>>> t.index('one')
0
```

```python
>>> t.count('one')
1
```

```python
>>> t = (1,1,2,3)
```

```python
>>> t.count(1)
2
```

Tuples are immutable


```python
>>> l = [1,2,3]
>>> print l
[1, 2, 3]
```

```python
>>> t = (1,2,3)
>>> print t
(1, 2, 3)
```

```python
>>> l[0] = 'string'
>>> print l
['string', 2, 3]
```
## Sets

An unordered collection of *unique* objects

```python
>>>  x = set()
>>>  x.add(1)
>>> print x
set([1])
```

```python
>>> x.add(2)
>>> print x
set([1, 2])
```

```python
>>> x.add(1)
>>> print x
set([1, 2])
```

```python
>>> # can use the set function to cast a list into a subset of unique elements
>>> l = [1,1,1,2,2,2,2,2,3,3,3,3]
>>> print l
[1, 1, 1, 2, 2, 2, 2, 2, 3, 3, 3, 3]
```

## Booleans

True / False / None

can be created as the results on conditional operators


# Flow of Control

## Using "If's"

## Looping with "for" loops

# Functions

##  Using Built-in Functions

If we want to use other mathematical functions, such as trigonometric functions or 
essentially anything more complex than arithmetic, then we'll need to import the functions from Python's **math** package.

By itself, the core Python language is pretty simple. Fortunately, however, there are an enormous number of packages which are available which incorporate additional functionality. We'll come back to this later in more detail, but for now let's just introduce this concept so that we can use

## Defining Your Own Functions

##  Adding Additional Functions using Packages

If we want to use other mathematical functions, such as trigonometric functions or 
essentially anything more complex than arithmetic, then we'll need to import the functions from Python's **math** package.

By itself, the core Python language is pretty simple. Fortunately, however, there are an enormous number of packages which are available which incorporate additional functionality. We'll come back to this later in more detail, but for now let's just introduce this concept so that we can use
