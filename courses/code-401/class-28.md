# CLASS 28 NOTES

## useEffect hook

### What is the main intended use case for the useEffect hook?

synchronize with some kind of external system

let you specify side effects that are caused by rendering, rather than by an event

- control non-react component based on React state
- set up server connection
- send analytics log

### How does the effect’s logic interact with the component?

- when the component is added to the DOM, React runs the setup function
- the setup function contains the Effect's logic
- after a re-render with changed dependencies, React runs cleanup function (if present)
- then re-runs setup function with new values
- after component is Removed from DOM, React runs cleanup function one last time

### What is the importance of the return value from the effect’s logic function?

the logic function should return the cleanup function, that should stop or undo whatever the Effect was doing

when the logic function runs again, it should be indistinguishable from the first run

running clean-up helps make this happen
