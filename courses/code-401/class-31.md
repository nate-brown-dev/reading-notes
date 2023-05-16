# reading 31 notes

## Choosing the State Structure

### Summarize the five principles for structuring state

1. group related state: if 2 state variables are updated at the same time, you might be able to group them into a single variable

2. avoid contradictions in state: don't have multiple state variables that can't be set to an impossible condition (contradictory booleans for example). instead, use a single state variable that has multiple possible conditions rather than booleans

3. avoid redundant state: if you can get some information from props or from other state variables, don't make a new state variable that uses that information. get the information from its other sources instead

4. avoid duplication in state: instead of defining an item in 2 places, have state reference the original item directly

5. avoid deeply nested state: make the state flat instead. also, move epheremal UI state to child components if it doesn't need to be stored

## Passing State Deeply with Context

### What problem do Contexts aim to solve?

contexts can allow a parent element to pass data to all of the child components in a tree, without requiring drilling props individually

1. ensures that all the components can get the data for maintenance etc
2. saves complexity

### What is one technique to try before useContext?

pass props normally - if you only have a limited number of props that you want to pass

### What hook complements useContext for complex applications?

useReducer can be combined with useContext to scale up complex applications

