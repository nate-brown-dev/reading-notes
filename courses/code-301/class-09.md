# Code 301 Reading 9

## Functional Programming Concepts

### What is functional programming?

- functional programming is a programming paradigm...that treats computation as the evaluation of mathematical functions and avoids changing state and mutable data
  - source: wikipedia article, quoted at [https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa]

### What is a pure function and how do we know if something is a pure function?

- a pure function does 2 things
  - it returns the same result if passed the same arguments
  - it does not produce observable side effects

### What are the benefits of a pure function?

- easy to test
- stable, consistent, predictable
- isolated from other parts of system/program

### What is immutability?

- immutable data cannot be changed after it's created
- if you want to change it, you create a new version of it that incorporates the changes, without changing the original value/element/object

### What is Referential transparency?

- when a function yields the same result for same input, is referentially transparent
- pure function + immutable data = referential transparency

## Node JS Tutorial for Beginners #6 - Modules and require()

### What is a module?

- a module is a part of a Javascript application that has a specific function
- splitting the javascript app into modules makes the application easier to understand and maintain

### What does the word ‘require’ do?

- it 'requires' the app to import the module that we are trying to use

### How do we bring another module into the file the we are working in?

- use 'require' in the importing app like `require './module'`

### What do we have to do to make a module available?

- use 'export' in the module with `module.exports`

[Go back home](/reading-notes/)
