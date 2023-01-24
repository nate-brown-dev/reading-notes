# Code 201 Reading 2

## HTML

### Why is it important to use semantic elements in our HTML?

- Semantic elements give meaning to the page that is recognized by the browsers and search engines
- This is important for accessbility (screen readers) and SEO

### How many levels of headings are there in HTML?

- There are 6 heading levels from `<h1>` (largest) `<h6>` (smallest)

### What are some uses for the `<sup>` and `<sub>` elements?

- `<sup>` and `<sub>` are necessary for writing some scientific and math expressions
- C<sub>6</sub>H<sub>6</sub>
- x<sup>3</sup>
- also for writing some date formats, although I never write dates that way (ie Jan 25<sup>th</sup>)

### When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term?

- must include the attribute `title` inside the leading `<abbr>` tag
- like this `<abbr title="Mlle">Madamoiselle</abbr>`

## CSS
 
### What are ways we can apply CSS to our HTML?

- inline (`style="somestyle"` attribute, in HTML element)
- internal (`<style>` element, located in HTML `<head>`)
- external (externally hosted file, referenced with `<link>` in HTML `<head>`)

### Why should we avoid using inline styles?

- internal styles make site maintenance difficult and time/labor intensive
- they make code hard to read as the CSS is mixed with HTML

### Review the block of code below and answer the following questions:

``` css
   h2 {
     color: black;
     padding: 5px;
   }
```

- What is representing the selector?
  - `h2` is the selector

- Which components are the CSS declarations?
  - `color`
  - `padding`

- Which components are considered properties?
  - `black`
  - `5px`

## JavaScript

### What data type is a sequence of text enclosed in single quote marks?

a `'string'` is enclosed in single or double quote marks

### List 4 types of JavaScript operators.

- arithmetic, assignment, logical, conditional

### Describe a real world Problem you could solve with a Function.

- the function can take user input and verify that it meets certain conditions, or else request it again

### An if statement checks a __ and if it evaluates to ___, then the code block will execute.

- checks a `statement`
- executes if the statement evaluates to `true`

### What is the use of an else if?

`else if` allows the statement to be evaluated for multiple `true` conditions

### List 3 different types of comparison operators.

- `==` equal
- `===` strict equal
- `!=` not equal

What is the difference between the logical operator && and ||?

- `&&` both statements must be `true`
- `||` at least one statement must be `true`

[Go back home](/reading-notes/)
