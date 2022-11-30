# Code 102 Reading 7

## Control flow

- What is control flow?
  - Order in which computer executes statements
  - Normally runs first to last
  - First to last can be changed with conditionals and loops

## Functions

### What is a function?

- Block of code to perform a task
- Run/executed when function is “called”

### Function syntax

``` javascript
function name(parameter1,p2,p3) {
// function code
}
```

- Function parameters in parentheses in function definition (local variables)
- Function arguments are passed to function when invoked
- Function executes when invoked/called
- Function stops when JS receives `return` statement
- Functions can be reused
- Functions can be used like variables in calculations

- Variables declared within function become local to function
- Can’t be accessed from outside

## Javascript operators

Assignment operator `=`
Assigns value to variable
NOT THE SAME as `==` or `===`

`+`  
`-`  
`*`  
`**`    power/exponent  
`/`  
`%`     modulus/remainder  
`++`    increment  
`—`     decrement  

Other assignment operators

`+=` x+=y | x = x+y  
`-=` x-=y | x = x-y  
`*=` x*=y | x = x*y  
`/=` x/=y | x = x/y  
`%=` x%=y | x = x%y  
`**=` x**=y | x = x**y

Adding strings

“String1” + “ “ + “string2” = “string1 string2”

### Concatenation of strings plus text

``` javascript
let x = word;
x += " salad" = "word salad"
```

- Adding string to number = number with concat string
- Adding numbers to string = all numbers are added as strings
  - String1 + 3 + 5 = string135

### Comparison operators

`==`    equal to  
`===`   equal value/type  
`!=`    not equal to  
`!===`  not equal value/type  
`>`  
`<`  
`>=`  
`<=`  
`?`     Ternary operator

### Logical operators

`&&`    logical and  
`||`    logical or  
`|`     logical not

### Type operators

`typeof`  
`instanceof`

[Go back home](/reading-notes/)
