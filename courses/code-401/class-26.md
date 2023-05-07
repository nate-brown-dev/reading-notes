# Code 401 Reading 19

## React Quick Start

### What are the building blocks of a React app?

Components

### What is the difference between an HTML element and a React component?

- React component is written with capital letter, HTML all lower case
- React component is written in Javascript instead of HTML
- React component is either class component or functional component

### What is JSX and why do we use it?

JSX enables writing markup in Javascript

### Describe the process of embedding JavaScript expressions in JSX.

Inside the markup (html/jsx) you can "escape back" to Javascript by using curly braces { }

You can also embed JS in JSX attributes the same way

### Does React or JSX have any special features for iteration or conditional logic?

- React uses the same conditionals as Javascript
- ? and && are common condition rendering methods in JSX

- For iteration, every item in a list has to have a "key" attribute/prop that is unique to the list item

### How does React know to respond to a user’s inputs?

React components can have event handler functions inside them

### What word indicates that a React component manages data with a Hook?

`use` at the start of the name indicates that the function is a Hook

### How can two react components share data?

React components share data by passing `state` and `props`

`state` gets passed from child component up to the parent component, and `props` get passed from parent component to child component

## Render and Commit

### What are the three steps of refreshing a React UI?

1. trigger a render
2. render the component
3. commit to the DOM

### How do you trigger updates to a component after the initial render?

after initial render, re-renders can be triggered by updating component state

### Does React recreate DOM nodes on every rerender?

React only changes DOM nodes if there is a difference between renders

### After React has updated the DOM, what still needs to happen before the user sees the change?

"browser painting" still has to happen before the user sees anything different

"browser painting" is actually browser rendering but is called "painting" to distinguish from React rendering

[Go back home](/../reading-notes/)
