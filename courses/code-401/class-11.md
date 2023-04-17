# Code 401 Reading 11

## Event Driven Programming

### What native Node.js module allows us to get started with Event Driven Programming?

- event emitter

### What is the value of Object Oriented Programming used in tandem with Event Driven Programming?

- this combination allows events to broadcast that they occur (emitting)
- then any object with a listener for that particular event observes the emitted event and takes action

### Consider your knowledge of Event Driven Programming in the Web Browser, now explain to a non-technical friend how Event Driven Programming might be useful on the backend using Node.js

- soundcloud
- creator posts a new mix to cloud
- event is emitted: new mix posted
- user that follows creator has event listener for new content from creators that user is following
- new post handler is triggered
- new mix is added to user's feed

[Go back home](/reading-notes/)
