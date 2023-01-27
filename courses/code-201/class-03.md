# Code 201 Reading 3

## Lists

### When should you use an unordered list in your HTML document?

- Unordered lists are for anything that does not require numerical/alphabetic order

### How do you change the bullet style of unordered list items?

- correct way is to use CSS list-style-type property
- deprecated way is to use attribute `type`

### When should you use an ordered list vs an unorder list in your HTML document?

- when the items must be shown in some kind of order (ie numeric)

### Describe two ways you can change the numbers on list items provided by an ordered list?

- CSS list-style property
- 'type' attribute
  `<ol type"i">`

### CSS

- "margin" and "padding" are the security detail for a secret government facility.
- "margin" surrounds the outer perimeter and the width of the margin is full of robot guard dogs who named Spike 1 to Spike 10 depending on the width of the margin.
- "border" is the outer perimeter fence.
- "padding" is between the outer and inner perimeters and it is full of angry cyborg beavers named Chompers 1 to Chompers 10 depending on the width of the padding. Inside the inner perimeter is the facility.
- "content" is the contents of the facility.

## JS

### What data types can you store inside of an Array?

- strings, numbers, objects, other arrays, other things too?

### Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?

- yes, you have to call the name of the array as a variable and reference the value you want
- `people([[1]])` returns `32`

`const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];`

### List five shorthand operators for assignment in javascript and describe what they do

`x = f()` -> x = f(x)
`x += f()` -> x = x + f(x)
`x -= f()` -> x = x - f(x)
`x *= f()` -> x = x * f(x)
`x /= f()` -> x = x / f(x)

### Read the code below and evaluate the last expression and explain what the result would be and why

 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;

### Describe a real world example of when a conditional statement should be used in a JavaScript program

- conditional statements can be used to respond to user input with multiple response possibilities

### Give an example of when a Loop is useful in JavaScript

- loop can be used to repeat an action a specific number of times with a counter

[Go back home](/reading-notes/)
