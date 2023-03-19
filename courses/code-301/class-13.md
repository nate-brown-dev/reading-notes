# Code 301 Reading 13

## CRUD Basics

### Which HTTP method would you use to update a record through an API?

- the proper HTTP methods to update a record are PUT and PATCH
- PUT replaces an entire object with an updated object
- PATCH changes the same object

### Which REST methods require an ID parameter?

- PUT and DELETE are examples of HTTP methods that require an ID parameter

## Video: Speed Coding: Building a CRUD API (Watch a Twitch streamer code an Express API in 20 minutes!)

### What’s the relationship between REST and CRUD?

- CRUD is a word that can use used to describe the basic functions in the server-client relationship of a REST API
- CRUD is its original meaning refers to functions required to complete utilize a database
- however these functions map over to using a web REST API
- the HTTP methods incorporated by a web REST API use the CRUD functions with different names

### If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

referenced these steps on restfulapi.net [https://restfulapi.net/rest-api-design-tutorial-with-example/]

1. identify the resources
   a. use an object model

2. create model URIs
   a. based on resource idenfication in previous step
   b. URIs should be nouns only

3. determine resource representations
   a. variety of resource representations

4. assign HTTP methods
   a. map the application's possible operations to the predetermined resource URIs

5. perform other actions
   a. logging
   b. security/authentication
   c. discovery

[Go back home](/reading-notes/)
