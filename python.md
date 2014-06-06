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


One space around an assignement or other operator
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

### References

[PEP 8, Style Guide for Python Code] (http://legacy.python.org/dev/peps/pep-0008/) 




