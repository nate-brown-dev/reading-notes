# Reading 36 Notes

## Dan Abramov Redux Tutorials

### What is the first principle of Redux?

quote:

The first principle of Redux is whether your app is a really simple one like this counter example, or a complex application with a lot of UI, and change of state, you are going to represent the whole state of your application as a single JavaScript object.

source: 0:00 at https://egghead.io/lessons/react-redux-the-single-immutable-state-tree

### what is a store and what do we use our reducers for within that store?

the store is the object that holds the state

the reducers in the store are used to manage application state

## Name three Redux store methods given to us by createStore and describe their use

- get state: returns the current value of the state variable

- dispatch: dispatching an action is the only way to change internal state

- subscribe: pushes new listeners into the listeners array

## Explain to a non-technical recruiter what combineReducers() does and why it is useful

the combineReducers function centralizes control of independent reducers functions.

each independent reducer has initial state and the combined reducer adds these states together to get application state.

each reducer is only responsible for updating part of the state on its own. the combined reducer can have the sub reducers update their piece of the state independently.

the whole process builds a "state tree" with the combined reducer as the trunk, and the other reducers as branches, and individual bits of state as leaves.
