javascript_cheat_sheet
======================

Quick Javascript guide; notes that I've taken primarily from working through Codecademy's JavaScript tutorial, and from Stack Overflow.

# Data types
**Primary (primitive)**: numbers, strings, Booleans (true, false)

**Composites**: objects, arrays

**Special**: null, undefined

# Arrays
Store lists of data (can be different data types); ordered

    var someArray = [item1, item2, item3];
	
Access elements, e.g.

    someArray[0] // first element

# Formatting
End statements with semicolon.

Comments: `//`

Single quotes, double equivalent.

# Make things appear in windows or log
Make box appear containing value:
`alert(value);`

Make confirmation box appear containing value:
`confirm(value);`

Prompt user for input:
`prompt(value);`

Print something to console:
`console.log(value);`

# Comparison
`===` strict equal to

`!==` strict not equal to

`&&` AND

So, to check `variable` is in the (inclusive) range of value1 and value2:

    if (value1 <= variable && variable <= value2) {...

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

# For loop

    for (var i=1; i < 10; i++) {
        statements
    }

Can iterate over arrays too:

Set the condition to be the length of the array and access the current element of the array with e.g. `someArray[i]` e.g.

    for (var i = 0; i < someArray.length; i++) {
        console.log(someArray[i]);
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

# Math(s)
Choose a floating point number between 0 and 1: 
    
    Math.random();
	
# Increment/decrement by 1 or n

    i++ 
    i--
    i += n
    i -= n

	(not really recommend outside of for loops)
