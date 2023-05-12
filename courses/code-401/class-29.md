# reading 29 notes

## Extracting State Logic into a Reducer

### What is the motivation for adding a reducer?

consolidate state logic into a single place

### What are actions in the context of a reducer? How are they different than setting state directly?

actions are objects that are sent (dispatched) to the reducer with data indicating how a task was acted on by an event handler

### What common list operation is useReduce named for, and why?

Array Reduce

Reduce takes an array and collapses it down to a single element, by performing an operation on each element in sequence (adding them together, or keeping/discarding based on some comparison criteria)

### When should you switch from useState to useReducer?

- if you have a lot of event handlers that modify state
- if state updates are complex
- if you have a lot of useState and there is a bug, you have to search through different components until you find it
- if you need to test state logic in isolation
- if you like reducers, some people just don't like them
