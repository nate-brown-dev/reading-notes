# Notes go here

## Code 301 Reading 12

### Status Codes Based On REST Methods

### In your own words, describe what each group of status code represents

- 100’s = informational
  - these codes report successeful receipt of request, along with some information about what the server will do with the request, but without reporting that the request was actually successful or unsuccessful
- 200’s = success
  - these code are for successful requests, for which the server is able to return requested resources
  - the request was accepted and the server is processing
- 300’s = redirection
  - these codes are for requests that have to be re-routed to another server because the server the request was sent to, no logner has the requested resource
- 400’s = client errors
  - these codes are for invalid requests that are broken in some way
  - time out
  - wrong URL
  - unauthorized
- 500’s = server errors
  - these codes are for problems on the server side (the client request was ok but the server can't return a correct response)
  - server overloaded
  - client request causes server errors
  - unreachable proxy
  - client can re-try the same request and it might work

- What is a status code 202?
  202 = Accepted for asynchronous processing
- What is a status code 308?
  308 = Permanent Redirect, tells client to use another URL to access the resource
- What code would you use if an update didn’t return data to a client?
  204 = No Content, for put/patch requests that are successful and don't require sending response to client
- What code would you use if a resource used to exist but no longer does?
  410 = Gone, resource was either deleted or moved to unknown location
- What is the ‘Forbidden’ status code?
  403 = Forbidden, client does not have sufficient permissions to access the resource

## Video - Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

### Why do we need to pull our MongoDB database string out of our server and put it into our .env?

- when we deploy the server we want the mongoDB URL to be a hidden environmental variable
- replacing the mongo URL with a variable name simplifies this for later

### What is middleware?

- middleware is software that connects two independent web services
- the middleware we are using is Express and it connects our server to MongoDB

### What does app.use(express.json()) do?

- it parses incoming JSON data to put in a request body

### What does the /:id mean in a route?

- it means that the 'id' is a parameter for the route
- everything after the : is the parameter
- for us the 'id' corresponds to mongodb _id

### What is the difference between PUT and PATCH?

- PUT replaces an entire object with an updated version of it
- PATCH keeps the same object but applies changes to that object

### How do you make a default value in a schema?

- when you declare the schema, you can add a key-value pair for "default" along with the other key-value pairs

shown below, taken from Mongoose JS documentation [https://mongoosejs.com/docs/defaults.html]

` js
const schema = new Schema({
  name: String,
  role: { type: String, default: 'guitarist' }
});
`

### What does a 500 error status code mean?

- 500 means there is an error inside the server, that is the server's fault, not the client's fault

### What is the difference between a status 200 and a status 201?

- 201 means 'successfully created object' instead of just 'successful' as in code 200

[Go back home](/reading-notes/)
