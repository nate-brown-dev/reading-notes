# Code 201 Reading 13

## Local Storage and How To Use It On Websites

### Why would a developer use local storage for a web application?

- local storage allows the 'state' of a website to be maintained between browsing sessions
- when stored locally it doesn't require user to log in or have an account to maintain state like server side storage
- it allows files to be stored locally / cached to reduce web site loading times / bandwidth

### What information should not be stored in local storage?

- user information and activities shouldn't be stored without user knowledge
- it's ridiculous to say this in 2023, everyone's information is stored everywhere and it's impossible to avoid, local storage is the least of anyone's problems

### Local storage can store what type of data? How would you convert it to that type before storing?

- local storage stores everything in strings
- other data types can be converted to strings with special methods
- `JSON.stringify`
- `JSON.parse()`

[Go back home](/reading-notes/)
