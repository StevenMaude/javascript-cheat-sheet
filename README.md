javascript_cheat_sheet
======================

Quick Javascript guide; notes that I've taken from Codecademy and Stack Overflow.

Data types:
Primary (primitive): numbers, strings, booleans (true, false)

Composites: objects, arrays

Special: null, undefined

# Formatting
End statements with semicolon.

Comments: `//`

Single quotes, double equivalent.

# Make things appear in windows or log
Make box appear containing string:
`alert(value);`

Make confirmation box appear containing string:
`confirm(value);`

Prompt user for input:
`prompt(value);`

Print something to console:
`console.log(value);`

# Comparison
`===` strict equal to
`!==` strict not equal to

# Strings
Length of string: `"string".length;`
Substrings: `"string".substring(x, y);`

# Variables
Declare (create) a variable (case-sensitive, normally camelCase):
`var varName = value;`

Reassign variable:
`varName = anotherValue`

## Global versus local variables:
Declare variable outside a function; global, accessible anywhere
Inside a function; local, only accessible within function

`var` creates variable in current scope 

# Conditionals

    if (condition) {
        statements
    } else if (condition) {
        statements
    } else {
        statements
    }

# Functions
Can declare a named function:

    function someFunction(args) {
        statements
    }

This is defined at *script parse time* so can be called any time.

Often used is an anonymous function with a variable:

    var someFunction = function(args) {
        statements
    };

This is defined at *runtime* so can only be called after this line is executed.
