# Reading 38 Notes

## async actions

### Why use Redux middleware?

reducers are not supposed to do anything besides returning function values (pure functions)

but any real app has to do all of these things like console logs, file system operations, timers, http requests, etc

### Consider the Redux Async Data Flow Diagram. Describe the flow in your own words

the event happens (deposit $10) then it is received by the event handler, and then dispatched to the middleware. the middleware makes the API call which returns to the middleware and is received by dispatch, which takes it to the reducer and then state is updated

### How are we accommodating async in our Redux app?

"thunk" functions contain the async logic. they take dispatch and getState as arguments

## thunk middleware

### Why would you need redux-thunk middleware?

a normal redux store can only handle synchronous updates by dispatching actions, it requires using the middleware to operate asynchronously

### Redux Thunk middleware allows you to write action creators that return a ____ instead of an action

function

### Describe how any return value from the inner thunk function will be made available

the return value from the inner thunk function is available as the return value of dispatch.