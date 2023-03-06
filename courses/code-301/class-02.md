# Code 301 Reading 2

## React lifecycle

### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

- `render` happens before `componentDidMount`

### What is the very first thing to happen in the lifecycle of React?

- mounting the constructor

### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

- constructor
- render
- React Updates
- componentDidMount
- render (updates)
- React Updates (updates)
- ComponentWillUnmount

### What does componentDidMount do?

- componentDidMount handles network requests and initializes the DOM
- it can also handle setting up subscriptions

## React State Vs Props

### What types of things can you pass in the props?

- props are like function arguments

### What is the big difference between props and state?

- props are passed to component
- state is handled inside component

### When do we re-render our application?

- after changing state

### What are some examples of things that we could store in state?

- counters
- votes
- forms

[Go back home](/reading-notes/)
