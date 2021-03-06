---
topic: "Python: Types"
desc: "int, float, bool, str, list, etc."
---

# Types in Python

In Python, every piece of data we deal with has a type.

Some of the most basic types are:

* `int` for integers (e.g. `-42`, `0`, `3`, `4567`)
* `float` for numbers that have decimal points, (e.g. `3.14159`, `0.5`, `-67.0`,`1.0`, `6.0221409e+23`)
* `bool` for the special values `True` and `False`

Some commonly used types that involve collections of things are:

* `str` for sequence of characters (e.g. `'Chris'`, `'UCSD'`, `'Computer Science & Engineering'`, `'6th College'`)
* `list` for lists of items, where the items can be of any type, or a mix of types.  Examples:
    - `[6, 10, 4, 17]`
    - `['Revelle', 'Muir', 'Marshall', 'Warren', 'Roosevelt', 'Sixth']`
    - `['Chris','Diaz',9876544,True]`
* `dict` for dictionarires of items, which are associations of *keys* and *values*.  Examples:
     - `{ 'one' : 'uno', 'two' : 'dos', 'three' : 'tres' }`
     - `{ 'fname' : 'Phill', 'lname' : 'Conrad', 'pid' : 1234567, 'gpa': 3.77, 'isHappy' : True }`
 
There are additional types that are less commonly discussed in "introductory programming", but that may end up being useful.

Here are a few of them:

* `NoneType` is a special type used for the the value that gets returned from a function that, literally, doesn't
    return anything at all.   For example:

    ```python
    def returnsNothing(x):
        x = x + 1
    ```
    
    ```
    >>> returnsNothing(3)
    >>> type(returnsNothing(3))
    <type 'NoneType'>
    >>>
    ```
* `Unicode` for sequences of a [larger set of characters](http://www.unicode.org) (e.g. `u'四'`, `u'piñata'`).
    - A python file that contains these characters may need to have a [special comment at the top](https://www.python.org/dev/peps/pep-0263/) to avoid errors when compiling. 
    - Example special comment for unicode: `# -*- coding: utf-8 -*-` 

* `tuple` is similar to list, but the object created is *immutable*, 
    meaning it cannot be changed after it is initially created. 
