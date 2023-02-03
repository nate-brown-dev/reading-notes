# Code 201 Reading 10

## What Went Wrong? Troubleshooting JavaScript

### Name some key differences between a Syntax Error and a Logic Error

- syntax errors are things like spelling errors, incorrectly placed special characters, etc that can break code but aren't usually serious
- logic errors are when code is written in a way that runs, but the results aren't what you expect because isn't doing what you were attempting to make it do
- syntax errors can usually be fixed and identified easily (especially with spell check / syntax highlighting! :) )
- logic errors can be complicated to find and fix

### List a few types of errors that you have encountered in past lab assignments and explain how you were able to correct them

- just recently, my background image didn't work
  - it was because the image URL is in the CSS file, and I didn't point to ../img/img.png
  - i've never referenced an image from inside CSS folder before and didn't even think of this
  - this is a logic error because the page worked but the image didn't display
  - the browser was looking for the image exactly where I told it to, but it wasn't there
  - it was really hard to figure out what was happening because there were no error messages to read
- before that when I was building the table in CSS I made a lot of syntax errors while typing the variable names
- when I made the form today I had weird errors with some of the math before I used parseInt and parseFloat to fix my form input
  - my function would still attempt the math but somethings it would return "0" for the calculation. Not "NaN", but 0.
  - logic error

### How will this topic continue to influence your long term goals?

- hunting for bugs is really fun
- syntax errors not so much
  - going through and looking for that one missing curly brace isn't that great
- logic error bugs yes
- finding a logic error, and understanding why it's a bug and how to fix it, is really satisfying, and it makes feel like I understand so much more than I did before I figured it out

## The JavaScript Debugger

### How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development?

- it allows you to go through a program step by step to watch what happens to variables and inputs

### Define what a breakpoint is

- a breakpoint is a place you want to stop code from going forward/executing at

### What is the call stack?

- shows you what code executed before you got to where you are now (at a breakpoint)

[Go back home](/reading-notes/)
