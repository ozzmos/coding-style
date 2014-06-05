## Python

### Indentation

Do not use tabs to indent code.

Use 4 spaces per indentation level.  

### Continuation lines

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




