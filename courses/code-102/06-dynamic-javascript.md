# Code 102 Reading 6

## How do computers work video series

Thought the videos did a good job of illustrating how decimal/base 10 numbers, as well as alphabet characters, are converted to binary

Good illustration of logic gates NOT / AND showing exactly what these statements mean in binary terms

## 3 Javascript readings

JS can go in HTML file, or separate file, like CSS

External file recommended

In HTML, JS enclosed in `<script>` javascript `</script>` tag

## 1. JS input/output

- Alert
  - Shows pop up in browser
  - The simplest javascript demonstration
  - Not actually useful

``` javascript
<script language=“javascript”>
    alert(“alert text”);
</script>
```

- Write to document
  - Adds to / changes page content
  - No longer useful?

``` javascript
<script>
    document.write(“<h1>write something</h1>);
</script>
```

- Log to JS console
  - JS console part of browser but not normally displayed
  - cmd+opt+j

``` javascript
<script>
    console.log(“write on your console”);
</script>
```

## 2. JS input/output with prompt and confirm

- Prompt
  - Pop up window with text and fillable field
  - Requires declaring variable of field entry
  - Can then write stored contents of variable using document.write

``` javascript
<script>
    var name = prompt(“What’s your name?”, “”);
    document.write (“Hello”, name);
</script>
```

- Confirm
  - Asks yes/no question
  - Yes returns true, no returns false
  - If/else
  - Yes = if = 1
  - no = else = 0

``` javascript
<script>
    if (confirm(“do you like to eat watermelon?”)) {
        document.write(“so do I”);
    } else {
        document.write(“what’s wrong with you?”);
    }
</script>
```

## 3. Javascript variables

- 4 ways to declare variables
  - `var`
  - `let`
  - `const`
  - Using nothing (undeclared variables)
- `var` was used before 2015
  - For older browsers, must use `var`
- For general use use `const`
  - `const` means “constant”
- For changing values use `let`

Variables must have unique names (identifiers)  
Variable names are case sensitive

To declare

`var varName;`  this is undefined variable since has no assigned value  
`let varName;`

After declaring variable, assign value

`varName = “pugetSound”;`

Or assign value when declaring

`let varName = “pugetSound”;`

It is **good practice to always declare variables at beginning of script**

[Go back home](/reading-notes/)
