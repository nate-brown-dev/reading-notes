# Notes go here

## Code 301 Reading 5

## React Docs - Thinking in React

### What is the single responsibility principle and how does it apply to components?

- in javascript or any language really, the single responsibility principle means that a  function/object should do only one thing
- if the function or object needs to do multiple things, they should exist in separate helper functions that get called by the main function
- in React the principle gets extended to components
- a single React component should do one thing
- for higher level components (App/Main/etc), the pieces that comprise them get broken out individually

### What does it mean to build a ‘static’ version of your application?

- a static version of a React app passes data only with props (no state)
- the static version does not have any interactivity with the user
- building the static version requires more typing than thinking

### Once you have a static application, what do you need to add?

- after the static version of the app is working, then interactivity can be added
- interactivity is implemented with state, for data that changes over time
- add the interactivity requires more thinking than typing

### What are the three questions you can ask to determine if something is state?

1. is the data passed from a parent via props? (if yes, not state)
2. does it remain unchanged over time? (if yes, not state)
3. can you compute it based on any other state or props in your component (if yes, not state)

### How can you identify where state needs to live?

- state needs to live in a component above any other component that needs to use the state
- that component should be the "common owner" of the other components that use the state
- if that doesn't work, put state in its own component and put it somehwere above the others that use it

## Higher-Order Functions

### What is a “higher-order function”?

- a higher order function is a function that operates on other functions
- the higher order function can take the other function as an argument
- or the higher order function can pass another function as a return

### Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

`return m => m > n`

- the function returns `true` if m is greater than n
- the function doesn't do anything without being passed a first argument (m) which creates a lower order function that can then test if m > n

### Explain how either map or reduce operates, with regards to higher-order functions

- map takes a function as an argument and applies it to all the elements in an array
- the return of map is an array in which each elements has been passed to the lower order function
- this is exactly how a higher order function works, it takes a function as an argument

[Go back home](/reading-notes/)
