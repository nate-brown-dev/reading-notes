# Code 201 Reading 5

## HTML

### What is a real world use case for the alt attribute being used in a website?

- for readibility with very slow internet connections, like in remote areas

### How can you improve accessibility of images in an HTML document?

- give them meaningful alt text (that describes what's in the picture)
- make sure your image files are reasonably sized

### Provide an example of when the figure element would be useful in an HTML document

- the `<figure>` and `<figcaption>` can be used to combine a picture and caption
- like you would see in an old book "Fig.2: The gorilla's spleen" with a picture of a gorilla spleen

### Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community.

- A gif is a special type of picture file, that's used if you need to be transparent, or have short animation
- a png is a good type of picture file to use for high-resolution pictures like photos

What image type would you use to display a screenshot on your website and why?

- png or jpeg, depending on what my computer made and which file size was more suitable

## CSS

### Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge

- in the simplest terms possible, think of a page in a book
- `color` is the color of the letters on the page
- `background-color` is the color of the page

### Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

- look through the page for the themes of his blog
- find some kind of pictures that describe the themes in the blog
- then use these pictures to find color that's representative of the pictures
- use one of the color picker tools to zero in on a specific background color
- once background color is established, add some color to other page elements using the same pictures as reference and same tools

### What should you consider when choosing fonts for an HTML document?

- readability
- consistency throughout page
- font availability for multiple systems
  - if you have to use weird fonts, have appropriate backup that's more common
- consider use fonts in the "Microsoft common fonts for the web" group
- don't make your whole page in monospace like it's 1993

### What do font-size, font-weight, and font-style do to HTML text elements?

- font-size: defines character size
  - depending on the way it's defined can be absolute (pixels) or em/rem (relative to parent elements)
- font-weight: defines bold/light
- font-style: italics on/off

### Describe two ways you could add spacing around the characters displayed in an `<h1>` element

- you could put space characters between each normal character (bad idea)
- use CSS properties `letter-spacing` and `word-spacing` to get the spacing you want

[Go back home](/reading-notes/)
