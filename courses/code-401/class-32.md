# Reading 32 Notes

## Scaling Up with Reducer and Context

### How do useReducer and useContext work together to simplify state management in a React application? (At least two paragraphs of prose.)

When these two things work together, the State lives at the top level of the application, and from there it gets managed by the Reducer. The Reducer contains all of the State update logic. Using the Reducer helps declutter and simplify the State logic. However if child components need to update or access this State, which right now is only at the top level component, it has to get passed to them. Passing a lot of props to individual components is tedious and time consuming and in an app that has many components, maybe even hundreds, this gets silly fast.

The answer is to combine the Reducer with Context. Any component that needs to access or update the State that is managed by the Reducer does so by receiving the Dispatch from the Context. The Context makes the Dispatch available to all of the app's child components. These components can access and update the state, which still lives at the top level component, without having to receive state or functions that update state as props. This whole process can be refined even further by combining the Reducer and the Context into a single file.
