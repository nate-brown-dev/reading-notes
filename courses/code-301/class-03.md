# Code 301 Reading 3

## React Docs - lists and keys

### What does .map() return?

- array.map takes an array and returns an array with the values transformed by a function
- either callback, or an inline operation

### If I want to loop through an array and display each value in JSX, how do I do that in React?

- you put the array element in curly braces {}
- then you put that in the loop return for a list item, etc

### Each list item needs a unique ____.

- list items need a unique key

### What is the purpose of a key?

- the keys are so React can identify the item
- the key will not change even if React changes the content of the item

## The Spread Operator

### What is the spread operator?

- the spread operator splits an array into separate arguments

### List 4 things that the spread operator can do.

- use math on all the elements of an array, like adding them all together
- work with React state
- combine objects
- combine arrays
- copy arrays

### Give an example of using the spread operator to combine two arrays.

- `let combinedArray = [...array1,...array2]`

### Give an example of using the spread operator to add a new item to an array.

- `let addedArray = ['b',...'array3']`

### Give an example of using the spread operator to combine two objects into one.

- `let combinedObject = {...firstObject,...secondObject}`

## How to Pass Functions Between Components

### In the video, what is the first step that the developer does to pass functions between components?

- pass the function to person object as props

### In your own words, what does the increment function do?

- the increment function in the video updates state to add 1 to the count property of a person object instance, and triggers the render to run again

### How can you pass a method from a parent component into a child component?

- by including the method as props in the parents component

### How does the child component invoke a method that was passed to it from a parent component?

- the child component calls the function using "this"

[Go back home](/reading-notes/)
