# Code 201 Reading 8

## Flexbox

### Flexbox is designed for one-dimensional content. Explain what this means.

- the "dimension" of the flexbox is the main axis
- it is "one dimensional content" because the one dimension is the main axis of the content (inline = linear = one dimension)
- the flexbox is intended to make inline items break onto a new line if the viewport size would cause them problems
- instead of forcing them to squish to the viewport, the right most element depending on language breaks off

Explain the difference between the main axis and cross axis.

- the main axis is the content direction. for inline content it's the "line" of the inline
- the cross axis is the perpendicular directon to the main axis

How can using certain properties of flexbox negatively impact accessibility?

- setting the flex items to reverse direction may cause readers to interpret them incorrectly and put the content out of order
- `order`
- `row-reverse`
- `column-reverse`
- all these can cause problems

### What are some advantages of using flexbox over float?

- with flexbox you can force column sizes to be the same even if the content doesn't fill all the columns
- you can vertically center an element inside another element
- you can make children of a container take up the same amount of space each

### How does this topic connect with your long term goals?

- I think a lot of the future in computing is in the mobile space with wildly inconsistent screen/viewport sizes
- flexbox can help make traditional websites more effective on mobile
- my non-work computer use is 100% mobile and i'm probably not unique

[Go back home](/reading-notes/)
