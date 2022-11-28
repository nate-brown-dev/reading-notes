# Code 102 Reading 5

## CSS notes

### What is CSS?

CSS used to define styles of web pages  
Works in conjunction with HTML  
Rule based language - apply particular styles to particular elements or groups of elements

Selector = specifies element/group of elements to apply style to
Curly brace `{`  
Declarations= paired `properties` and `values`  
Close curly brace `}`

``` css
element {
    property1: value1;
    property2: value2;
}
```

Each property has its own set of acceptable values

### 3 ways to insert CSS

- External
  - External = external style sheet (separate file)
  - Referenced in HTML file `<head>`
  - Single style sheet for entire web site or section of web site
  - Written in text editor
  - `.css` extension

- Internal
  - For single HTML page with unique style
  - Defined with `<style>` element inside `<head>`

- Inline
  - Apply unique style to single element
  - `<h1 style=“color:color1;text-align:center;”heading1</h1>`

For contradictory overlapping styles  
Ie external style sheet + internal style in head + inline style  
Last one read will be displayed  
External and internal are both defined in `<head>`  
whichever of these comes last will be displayed  
Inline styles always supersede internal/external  
Browser default is last

### CSS colors

Color = property of text (text color)

``` css
body {
    color: #000000
}
```

Color: initial | inherit

Initial = keep certain elements inside other element to have originally specified color, not enclosing element color

``` css
div {
    color: red;
}

h1 {
    color: initial
}
```

Inherit = get color from enclosing/parent element

``` css
span {
    color: red;
}

.extra span {
    color: inherit
}
```

Only elements specified with class `.extra` will get the inherit color

### Ways we can specify color

- Hex = 6 alphanumeric digits 0-9+a-f
  - `#ff0000` = red
- Hex with transparency  
  - `#ff000080` = red transparency  
  - add 2 additional digits to hex color 00-ff
- RGB  
  - `rgb(255, 0, 0)` = red
- RGBA
  - Rgb with transparency / opacity
  - add 4th parameter 0.0 = fully transparent 1.0 = fully opaque
  - `rgba(255, 0, 0, 0.5)` = red w opacity 0.5
- HSL = color wheel
  - hsl(hue, saturation, lightness)
  - `hsl(120, 100%, 75%)`
- HSLA
  - HSL plus opacity like RGB
- Predefined
  - 140 colors in CSS/HTML spec
- `currentcolor` keyword

[Go back home](/reading-notes/)
