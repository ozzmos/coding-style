## Python

### Table of content

[Indentation](#indentation)  
[Maximum line length](#maximum-line-length)  
[Blank lines](#blank-lines)  
[Import] (#imports)  
[Naming conventions](#naming-conventions)  
[Whitespace in expressions and statements](#whitespace-in-expressions-and-statements)  
[Comments](#comments)  
[References](#references)

### Indentation

Do not use tabs to indent code.

Use 4 spaces per indentation level.  

### Maximum line length

Limit all lines to a maximum of 79 characters.  
Continuation lines should align wrapped elemenets vertically.

You can cut long text with an apostrophe
```
print('Lorem ipsum dolor sit amet, consectetur adipiscing elit.  Donec a'  
      ' diam lectus. Sed sit amet ipsum mauris. Maecenas congue ligula '
      ' ac  quam viverra nec consectetur ante hendrerit.')
```

You can also cut after a colon
```
foo = long_function_name(var one, var two,
                         var three, var four)
```

Or before a plus sign
```
print('Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec '
      + end_of_text)
```

### Blank lines

Class definitions and to-level function are separated by two blank lines.  

Method definitions inside a class are separated by a single blank line.  

### Imports

Imports are always put at the top of the file, after modules comments and docstrings and before module globals and constants.  

Imports should be grouped in the following order:  
1. standard library imports  
2. related third party imports  
3. local application/library specific imports  

Each group should be separated by a blank line.  

Do not use relative path but absolute path.   
```
from foo.bar.yourclass import YourClass
```

Import should usually be on a separate lines.  
```
import os
import sys
```

However it's okay to say:
```
from subprocess import Popen, PIPE
```

### Naming conventions

**variable** : lowercase, underscores can be used to improve readability  
```
firstname = 'Christophe'
```
**function** : lowercase, underscores can be used to improve readability  
```
def show_firstname():
```
**class** : use CapWords convention  
```
class UserTest(object):
```
**method** : lowercase, underscores can be used to improve readability  
```
def create_user(self):
```
**module** : short lowercase name, use of underscores is discouraged  
```
import busconnection 
```
### Whitespace in expressions and statements


One space around an assignement, augmented assignement(+=,-=,etc.) or other operator(==,<,>,!=,<>,<=,>=,in,not in,is,is not), Booleans(and,or,not).  
```
x = 1
if x == 4:
```

One space after a colon
```
def test(self, name):
```

### Comments

Should be a complete sentence. If a comment is a phrase or a sentence, its first word should be capitalized.

#### Inline comments

Use inline comments sparingly  
Should be separated by at least two spaces from the statement  

#### Block Comments

Block comments generally apply to some(or all) code that follows them, and are indented to the same level as the code. Each line of a block comment starts with a # and a single space.  

Paragraphs inside a block are separated by a line containing a single #.  

### Documentation Strings

A docstring is a string literal that occurs as the first statement in a module, function, class or method definition.
This becomes the __doc__ attribute of the object.

Docstrings should be written for every public module, function, class or method and describe what it does.  
A package may be documented in the module docstring of the __init__.py file in the package directory.  

Always use triple double quotes around docstrings.  

One-line docstring:  

```
def kos_root():
    """Return the pathname of the KOS root directory."""
    global _kos_root
    if _kos_root: return _kos_root
    ...

```

Multi-line docstring:  
```
def complex(real=0.0, imag=0.0):
    """Form a complex number.

    Keyword arguments:
    real -- the real part (default 0.0)
    imag -- the imaginary part (default 0.0)
    """
    if imag == 0.0 and real == 0.0:
        return complex_zero
    ...
```


### References

[PEP 8, Style Guide for Python Code] (http://legacy.python.org/dev/peps/pep-0008/) 
[PEP 257, Docstring Conventions] (http://legacy.python.org/dev/peps/pep-0257/)




