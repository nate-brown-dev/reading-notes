# Reading 37 Notes

## Multiple Reducers Example

### Why create multiple reducers?

using multiple reducers simplifies code maintenance and makes the application less complicated by dividing responsibility among smaller components

### How would you combine multiple reducers?

reducers are combined with the Redux `combineReducers` function

### How will you manage state as an immutable object? why?

the state object is managed by replacing the whole state object with new state instead of mutating the old state

mutating state is a big nono in React!!

## Redux Docs: Using Combined Reducers

### combineReducers is a utility function to simplify the most common use case when writing ____

Redux reducers

### Explain how combineReducers assembles the new state tree

each reducer has a piece of the global state object that belongs to it

when the new state tree is assembled, combineReducers calls each slice reducer and gets its piece of the state

then the new state object is assembled and state is updated

### How would you define initial state in an app using combineReducers?

the createStore function can accept preloaded state as a second argument from local storage

OR the root reducer can return the initial state value when the state argument is undefined

## Redux Docs: Combined Reducer Syntax

### Why will you want to split your reducing functions as your app becomes more complex?

otherwise the state object will become impossible to manage by a single reducer as the state object contains values

### The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____

combineReducers, createStore

### What is a popular convention when naming reducers?

reducers are named after the state slices that they manage