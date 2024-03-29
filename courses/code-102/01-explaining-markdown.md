# Reading 1: Explaining Markdown

## Transcript of Friday's discussion with N.T.F

> [@non-technical-friend](mailto:non-technical-friend@seattle.gov) wrote:  
>
> What exactly is Markdown?

Markdown is a tool to generate web pages by writing them in a form of shorthand or "syntax".

> Ok, so what is it good for?

Markdown allows the writer to focus on the content of the pages rather than on the time-consuming and technical process of writing them in HTML.

> What's HTML?

HTML is the language of web pages. After a creator produces a page using Markdown, GitHub converts the Markdown syntax into HTML that can be read by any web browser application.

> So it can be used to create fully featured web pages?

Not exactly. The Markdown syntax is not intended as a replacement for HTML and its feature set is intentionally limited. It's best for pages that only require text and simple images, kind of like the the pages you remember from growing up in the 1990s.

> Yes, I remember those. Now how do I create a page with it?

In your GitHub repository, click the button for `Add file` and select `Create new file`. This will immediately send you to a page with a large text box and a field to enter the file's name.

> How does GitHub know that I'm going to use Markdown?

When you name the file, it's important to include the extension `.md` at the end of the file name. This extension indicates to GitHub that it needs to read the text box as Markdown so it can be converted to HTML later.

> What happens if I forget to add .md to the file name?

If you write a bunch of Markdown in the box but don't include the `.md` extension, you'll get a messy, unformatted wall of text with Markdown symbols mixed in everywhere. You can check this easily by clicking the `Preview` tab at the top of your text box.

> I'm ready to start working on my page. How do I add a title at the top?

Markdown has 6 levels of headings for breaking content into sections. To set a line as a heading, include from 1 `#` to 6 `######`characters in front of the line, followed by a space:

`## Heading Level 2`

Two `##` is the second-largest heading so you'll want it for your title. It displays like this:

## Heading Level 2

The other heading levels work the same way, just remember that the more `#` characters you use, the smaller the headings get, like so:

`#### Heading Level 3`

### Heading Level 3

And remember, there is no heading level 7 so don't try to use it!

####### isn't a thing in Markdown

> That's enough about headings. What else can I do with my text?

Markdown supports **bold**, *italic*, ~~strikethrough~~, **bold *nested* italic**, ***all bold italic***, subscript '< sub >', and superscript '< sup >'. See **bold** here:

`**bold text**` will make **bold text**

I'll let you look the rest up on your own.

> Fair enough. How do I add a picture?

For simplicity's sake we'll pretend there is already an image file in your repository named `octopus.png`. You can display this image using a relative link (which references a file already in the repository) like this:

`![Silly octopus](octopus.png)`

![Silly octopus](octopus.png)

You could also use an absolute link that references an externally hosted file. However absolute links can break easily as hosting websites change, so this may not be a good idea.

> One last thing, how do I link to other pages?

There are a few different ways of writing links in Markdown.

One way uses square brackets `[]` and parentheses `()` like so:

`[Google](https://www.google.com/)` [Google](https://www.google.com)

You can also select some text, push `Cmd+K (on Mac)`, and pasting the link. This method automatically creates the brackets and parentheses for you.

> Thank you, that's as much info as I can absorb in for one afternoon. I'll get to work writing pages very soon!

You're welcome 🍻

[Go back home](/reading-notes/)
