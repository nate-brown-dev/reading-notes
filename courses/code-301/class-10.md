# Code 301 Reading 10

## Understanding the JavaScript Call Stack

### What is a ‘call’?

- a call is a function invocation

### How many ‘calls’ can happen at once?

- 1, javascript is single threaded (one function executes at a time)

### What does LIFO mean?

- last in first out
- the last function pushed into the stack is returned first
- this way functions above the last function in the stack can use the return of the last function

### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack

` js
function function1() {
  function2();
}

function function2() {
  console.log('hello from function 2');
}

function1();
`

### What causes a Stack Overflow?

- when a recursive function calls itself without an exit point
- there is a maximum stack call, when the browser reaches it, there is a stack error

## JavaScript error messages

### What is a ‘reference error’?

- using an undeclared variable
- using let and const in some circumstances before they are hoisted (TDZ)

### What is a ‘syntax error’?

- when programming syntax cannot be parsed
- parsing = converting written code to machine language in a compiler, or converting to data structures, etc

### What is a ‘range error’?

- trying to use a number that is not in the possible range for the input
- example arrays can't have length less than 0

### What is a ‘type error’?

- trying to use an element of incompatible type (object/number/etc)
- trying to use element that is undefined if undefined is not possible type

### What is a breakpoint?

- a place where you can stop a program from running while using a debugger so you can analyze the lines after it

### What does the word ‘debugger’ do in your code?

- it allows you to see the "history" when running that code before the breakpoint
- it shows the call stack at that point

[Go back home](/reading-notes/)
