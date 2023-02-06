# Code 201 Reading 11

## Video and Audio Content

### Explain how the ability to use video and audio on the web has evolved since the early 2000s

- I can answer this from memory as I lived it :)
- back then, playing video on web pages required special plug ins that did not work very well
- before Flash and Silverlight there was "Real Player"
- Shockwave Flash came before Silverlight
- all of these were frustrating to use and crashed a lot
- now we can directly embed video with HTML tags

### Describe the use of the src and controls attributes in the `<video>` element

- src element = same as for pictures
- controls attribute shows browser default video controls

### Why is it important to have fallback content inside the <video> element?

- fallback content has two uses
  - if browser doesn't support embedded video, can show direct link
  - if video doesn't work, there's something to show instead

Write a very short story where <audio> and <video> are characters.

- Audio and video are best friends. In the beginning of the internet, neither one worked on web pages, or anywhere else really. You had to request their presence by "downloading" them and there was a good chance they wouldn't show up, or show up too wasted to perform. Other times they would like to "crash" at unsuspecting computers when the users didn't know what they were downloading, or were trying to download something sketchy. Mostly they were too busy hanging out with their friends in the music industry and Hollywood. This was because the internet was too slow for them, and they like to live fast, especially video. But after many years of improvements to the internet infrastructure, now they use up most of the internet's bandwidth, and even Hollywood video appears on the internet before it appears anywhere else.

## A Complete Guide To Grid

### How does Grid layout differ from Flex?

- flex flow only in one direction (flex main axis)
- grid has columns and rows

### Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.

- the grid container contains all of the grid elements, just like the flex container contains the flexing elements.
- grid items are the direct children of the grid containers
- grid lines are the horizontal and vertical lines between grid cells
- grid cells are the individual boxes where the grid content goes
- grid cells can be combined (spanned) across rows and columns

### Responsive Images

### Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

- saves bandwidth on mobile
- can make pages more viewable/higher quality on desktop

### Define the following <img> attributes srcset and sizes. Write an example of how they are used.

- example: I have 3 images
- srcset: is a set of all these images
  - 400x400, 800x800, 1200x1200
- sizes: defines conditions for which each size will be displayed
  - 400x400 on low fidelity mobile
  - 800x800 on high resolution mobile
  - 1200x1200 on desktop
- more specifics than that but general idea

How is srcset more helpful for responsive images than CSS or JavaScript?

- srcset runs during HTML load of page, before the page has implemented any CSS/JS
- images start downloading immediately during HTML load
- changing image sizes with CS/JSS is too late because they have already downloaded, so it doesn't save bandwidth

[Go back home](/reading-notes/)
