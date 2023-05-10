# CLASS 27 NOTES

## Thinking in React

### Summarize the five steps of thinking in react

1. break up the UI into component hierarchy: draw them, or go from css names, or whatever
2. build static version in react ( static = props only, no state )
3. find minimal representation of UI State: least amount of state to operate the interactivity you want
4. identify where state should live: figure out who owns the state
5. add inverse data flow: allow child components to change parent state

## State: A Component’s Memory

### What is one reason a local variable isn’t sufficient for managing a React component?

local variables don't persist between renders

### What is the argument to the useState hook, and what are the two parts of its return array?

argument passed to hook: initial value of state variable

two parts of return array:

1. state variable with value you stored
2. state setter function which can update variable and trigger re-render

### How can Component A access state from Component B?

component B can pass state data to a shared parent and then the parent can pass to component A as props
