# CLASS 28 NOTES

## useEffect hook

### What is the main intended use case for the useEffect hook?

synchronize with some kind of external system

### How does the effect’s logic interact with the component?

- when the component is added to the DOM, React runs the setup function
- the setup function contains the Effect's logic
- after a re-render with changed dependencies, React runs cleanup function (if present)
- then re-runs setup function with new values
- after component is Removed from DOM, React runs cleanup function one last time

### What is the importance of the return value from the effect’s logic function?

the function returns undefined on the 1st render

state changes in react are asynchronous so it can't return anything besides undefined on the first render
