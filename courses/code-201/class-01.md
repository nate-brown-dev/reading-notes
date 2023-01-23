# Code 201 Read: Class 01

## Getting started

### 1. Compose a short poem describing how HTTP sends data between computers

Client queries server

Server replies with packets

Client parses answer

### Describe how HTML, CSS, and JS files are “parsed” in the browser

1. The browser parses (reads) the HTML file first and locates `<link>` and `<script>` tags
2. The browser requests any files associated with these tags (external CSS/JavaScript files)
3. The browser builds Document Object Model (HTML) tree and CSS Object Model (CSS) and compiles any JS scripts
4. The browser renders the page HTML, applies CSS to it, and executes scripts. HTML reads top to bottom, user starts to see page, browser continues until page completely loaded

### How can you find images to add to a Website

When using Google image search, select Tools > Usage rights > Creative Commons licenses, to find only images whose license explicitly permits use.

### How do you create a String vs a Number in JavaScript

- To make a string, enclose it with quotes `"string"`
- No quotes is a `number`

### What is a Variable and why are they important in JavaScript?

- a variable is a container that stores values
- the contents of the container are stored in the machine's memory and can be retrieved later by function calls
- the value of the variable can be assigned and then changed later

## Introduction to HTML

### What is an HTML attribute

An HTML attribute is a property that is assigned to an HTML element but does not appear in the content. The attribute is placed in the opening tag of the element like this:

```html
<element attribute="property">element</element>
```

A common attribute is `class`

### Describe the Anatomy of an HTMl element

- an HTML element has 3 parts
  - opening tag
  - content
  - closing tag

These parts are usually separated into 3 distinct parts like this

```html
<opening tag>content</closing tag>
```

However there are "self closing" tags that consist of a single piece

```html
<img src="source.jpg" />
```

note that the tag closes with space and backslash at the end

### What is the Difference between `<article>` and `<section>` element tags

I've read at least 5 different explanations of the difference between these two tags and I can't find any explanation that doesn't use self-referential definitions or circular logic.

`<section>` is used for separating parts of a page by function

`<article>` is used for separating bits of independently meaningful content

however an `<article>` can be divided into `<section>` (s) or a `<section>` can include multiple `<article>` (s)

### What Elements does a “typical” website include

- header
  - title of page / banner at top
- navigation bar
  - enables movement from one page to another in multiple page sites
- main
  - content of page
- sidebar
  - additional info related to content, or additional navigation
- footer
  - copyright info, author contact, legal notices, things most people don't read

### How does metadata influence Search Engine Optimization

- The information in the metadata is used when displaying search engine results as the page "title" and "content"
- however there are additional unused elements of the `<meta>` tag that are no longer used by search engines because of bad website/creator behavior

### How is the <meta> HTML tag used when specifying metadata

the `<meta>` tag can be used to define the author, describe the content, and specify the character set of the page

## Miscellaneous

### What is the first step to designing a Website?

the first step used by many web designers, after defining the purpose/content of the page, is to draw it out on paper/white board, before doing any work on the computer

### What is the most important question to answer when designing a Website?

- the question is "what do I want my page to do?"
- until this question is answered the page is just a meaningless, disordered collection of information

### Why should you use an `<h1>` element over a `<span>` element to display a top level heading?

`<h1>` is a semantic element, which means the browswer recognizes it as having organizational meaning (top level heading). `<span>` can be used to create an element that looks like that heading but doesn't carry the meaning.

### What are the benefits of using semantic tags in our HTML?

- as above, browsers recognize semantic tags
- search engines use semantic tags to categorize pages
- accesibility accomodations / page text to speech

### Describe 2 things that require JavaScript in the Browser?

- store variables
- respond to user input

### How can you add JavaScript to an HTML document?

- JS can be placed directly in the page with script tags, or referenced with external script file

## Things I want to know more about

HTTP status codes - "200 OK", relationship to 403/404 etc

[Go back home](/reading-notes/)
