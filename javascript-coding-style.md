## JavaScript

### Table of content


### JavaScript files

JavaScript files should be saved as *.js* files.  
The code should not be embedded in HTML files unless the code is specific to a single session.  
The JavaScript tag should be placed as late in the body as possible to reduces delays.  
No need to use the *language* or *type* attributes. They are determined by the server.  

### Indentation

Do not use tabs to indent code.

Use 4 spaces per indentation level.  

### Line length

Limit all lines to a maximum of 80 characters.

### Variable declarations

All variables should be declared before used. JavaScript does not require this, but doing so makes the program easier to read and makes it easier to deect undeclared variables that may become implied globals. Implied global variables should never be used.  

The var statements should be the first statements in the function body. Each statement on its own line with his given comment. 

List variable declaration in alphabetical order.  

Use of global variables should be minimized.  

Implied global variables should never be used. 
```
var a = 5;    // global variable 
x = 42;       // implied global variable 

function test() {
    var x;    // variable 
    var y;
    var z;
    …
}
```

### Function declarations

All functions should be declared before they are used.  

Inner function should follow the var statement.
```
function outer(c, d) {
    var e = c * d;
    
    function inner(a, b) {
        return (e * a) + b;
    }
    
    return inner(0, 1);
}
```

### Whitespace in expressions and statements

One space after a colon.  

No space between the name of a function and the left parenthesis.  

One space between the right parenthesis and the left curly brace.  

```
function test(a, b) {
}
```
