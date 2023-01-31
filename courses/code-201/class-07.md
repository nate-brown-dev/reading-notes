# Code 201 Reading 7

## Explain why we need domain modeling.

- domain modeling allows a concept to be tested in code
- allows stakeholders/teams/different groups to have mutual understanding of the problem and how to talk about it

## Tables

### Why should tables not be used for page layouts?

- tables don't work with screen readers/cause accessibility issue
- table layout is more complex than CSS and causes "tag soup"
- tables automatically size to content instead of parent element

### List and describe 3 different semantic HTML elements used in an HTML <table>.

`<td>` table cell
`<tr>` table row
`<th>` table headr

## Constructors

### What is a constructor and what are some advantages to using it?

- is a way of utilizing an object
- allows the object code to be reused
- doesn't require changing object code for many instances of similar object

### How does the term this differ when used in an object literal versus when used in a constructor?

- `this` for object literal is self-referential to that object
- `this` for constructor is for the named instance of the object

## Explain prototypes and inheritance via an analogy from your previous work experience.

### NOTE: This is a very common front end developer interview question

- for an infantry rifle squad, the prototype is defined in FM 7-8, a doctrine publication
- when local leadership assembles a squad out of actual soldiers, they do so based on the definitions in FM 7-8
- if something doesn't match, refer back to the prototype

[Go back home](/reading-notes/)
