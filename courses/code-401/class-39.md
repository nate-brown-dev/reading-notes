# Reading 39 Notes

## Redux Toolkit (RTK)

### What concerns are addressed by Redux Toolkit?

1. "configuring a redux store is too complicated"
2. "I have to add a lot of packages to get Redux to do anything useful"
3. "redux requires too much boilerplate code"

funnily enough all of these complaints are things I have seen posted on Reddit about Redux, but also about React Hooks in general

more generally RTK makes Redux "more opinionated" meaning that it provides a consistent way to approach using the tools and encourages them to be used in exactly that way. This makes using them in a way outside the "normal" way more complicated but it can make setup easier if you don't have those kind of specific requirements

### What does configureStore() do?

configureStore() wraps createStore() with simplified configuration options and defaults

automatically combines slice reducers

adds redux middleware and includes Thunk by default

### How would I use createSlice()?

To use createSlice, you supply an object of reducer functions, a name, and an initial state value, and it makes the slice reducer for you

## MobX

### What is Mobx?

MobX is a simple and scalable state management solution

### How does MobX make it “impossible” to produce an inconsistent state?

mobx has state, reactions, derivations, and actions

derivations are values that arise from function operations on state values
reactions are functions that don't return values, ex IO related function returns
actions are anything that alters state

Mobx makes sure that all the derivations and reactions occur anytime the state changes as the result of an action. it does this by automatically executing these derivations and reactions for any state change

### How would we build a reactive user interface?

to build a reactive user interface with mobx, you wrap the react component in `autorun` and make the component `observable`

## Tutorial

### What take-away(s) did this tutorial provide?

the goal of RTK is to simplify common Redux use cases

RTK configure store gives you

- an options object with named parameters
- Redux Devtools extension enabled automatically
- redux thunk added by default