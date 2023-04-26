# Code 401 Reading 3

## Review: ES6 Classes

### Classes are a template for creating ____

Objects

### Can a class declaration be hoisted?

No, class declarations go in the "temporal dead zone" like variables declared with let or const

### How would you describe a constructor and contextual “this” to a non-technical friend?

- A constructor is a template for creating an object
- "this" refers to the object that will be created, or to the object once it's created

- The object's properties are referenced with "this" like so:
- Object is a square, and......
- This square's color is...
- This square's sides are x cm long
- This square is made of...
- and so on

## Using Express Routing

### Within Express, what does routing refer to?

- Routing is how an app's endpoints respond to client requests

### What is the difference between a route path and a route method?

- route path = defines endpoint where requests can be made
- route method = defines type of request

### When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?

- if there are multiple callback functions associated with a request, can use next() as a parameter to pass to a callback
- next will bypass remaining callbacks on the route
- if next gets passed to middleware as parameter, the middleware needs to call next to pass control to the next middleware

## Express Routing

### What is an Express Router?

- Router is like a mini-express
- Provides Routing APIs like `.use` `.get` `.param` `route`
- All it does is routing

### By what mean do we initialize express.Router() in an express server?

- Initializing the router means calling the router instance so that it's active while the express server is running
- When the router is active, all traffic on its routes goes through it

### What do we use route middleware for?

- Route middleware allows requests to be examined before processing
- Requests can be validated and logged
- Requests can be checked for authentication/authorization
- Route middleware has to be placed in front of the routes in the server, so that the requests go through the middleware first
- If the routes are before the middleware, it doesn't get used because the requests go directly to the route

[Go back home](/../reading-notes/)
