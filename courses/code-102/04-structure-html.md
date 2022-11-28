# Code 102 Reading 4

Notes on wireframing and simple HTML tags

## Wireframing

Process of organizing UX before writing code by sketching, drawing on whiteboards, etc

Define how user interacts with site/product

Plain black and white diagrams

### Tools for wireframing

- White board
- Scratch paper
- Software (not going to use this today

### Wireframing steps

1. Do research
   - audience requirements
   - use cases
   - product analysis
   - competitor research
2. Prepare and organize research
3. Map user flow, information architecture
   - User flow
     - where users come from, marketing / socials / referrals etc
   - Information architecture
     - organization so users can find things without help
     - reduce customer service requirements for simple task help
4. Draft/sketch
   - make it down and dirty
   - not over detailed
5. Add detail and begin tests
6. Transition from wireframing to prototyping

### Wireframing principles

- Clarity
- Confidence
- Simplicity

## HTML tags

Paragraph `<p></p>`

Element = tag plus contents

Tag = signifies type of element, most elements have opening and closing tags

Attribute = non-visible property of element

Attribute has *name* and *value*

Class = type of attribute that is non unique identifier for element (for CSS)

`<p class=“class”>` content `</p>`

Nested elements: must be consistent, first open = last closed

Void elements = tag that closes itself, ends with />

### Basic html anatomy

`<!DOCTYPE html>` = required, from early days of html/web

`<html lang =“en-US”>` = root element, wraps all content

`<head>`

Everything that isn’t content on page

Keywords, page description for search, CSS, character set, etc

`</head>`

`<meta charset=utf-8>` = UTF-8 character set, preferred by HTML5

`<meta name=“viewport” content=“width=device-width”>`
Force page width for mobile

`<body>`

All page content goes here

`</body>`

`</html>` closing html tag, wraps everything

#### Images

`<img src=“url” alt=“text if image doesn’t load” />`

Unpaired tag, self closing

#### Headings

6 levels of heading, like markdown

`<h1>` largest, page title

`<h2>`

Etc

`<!— HTMLS comments look like this —>`

#### Lists

`<ul>` = unordered list

- `<li>`list item`</li>`
- `<li>`list item`</li>`

`</ul>`

`<ol>` = ordered list

1. `<li>`list item 1`</li>`
2. `<li>`list item 2`</li>`

`</ol>`

#### Hyperlinks

`<a href=“url”>` Link Name `</a>`  
href = hypertext reference

[Go back home](/reading-notes/)
