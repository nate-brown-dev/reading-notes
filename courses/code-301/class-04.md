# Code 301 Reading 4

## React Docs - Forms

### What is a ‘Controlled Component’?

- a form element whose value is controlled by the React component that renders the form

### Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

- I don't understand what this question is asking and the linked reading doesn't answer it
- the form input updates state with every key stroke but setState should go on submit

### How do we target what the user is entering if we have an event handler on an input field?

- the user input is stored in this.state.value

## The Conditional (Ternary) Operator Explained

### Why would we use a ternary operator?

- the ternary operator is a way to simplify 'if' statements

### Rewrite the following statement using a ternary statement:

` JS
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
`

`x === y ? true : false;`

I think that's it?

[Go back home](/reading-notes/)
