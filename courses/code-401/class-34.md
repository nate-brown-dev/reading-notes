# Reading 34 Notes

## Review API Server Build

### Explain the different between a query string parameter and a path parameter.

- path parameter points to a specific resource
- query string parameter is used to filter the results

- GET /pokemon gets all pokemon, this is a path parameter

- GET /pokemon?color=blue filters for blue pokemon, this is a query string parameter

### What would our API URL with a path id parameter be given the following information:

Domain: http://our-site.com
v3
model name: stuff
id: things

http://our-site.com/v3/stuff/things

### We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.

the interface consists of a web page that allows the user to access remote resources, like looking through a file cabinet without actually being in the room

## Review Auth Server Build

### Describe how you would use middleware to implement basic and bearer auth.

the middleware for basic and bearer auth is imported into the router module and from there is is passed as an argument to the route, ahead of req/res to make sure that authentication happens first

### Describe the handshake necessary to implement OAuth.

user requests resource from server, resource server redirects client to authentication server, client authenticates, authentication server generates token for client, client passes token to resource server, resource server gives resource access to client

### Describe how Role Based Access Control works to a non-technical friend.

role based access control: a user gets assigned a role (based on their job), and that role defines what things on the network the user can view, edit, or delete on the company's systems. If another person gets hired to do the same job, they get assigned the same role, and the new user can do exactly the same things. That's because the access capabilities (permissions) belong to the ROLE, not the user. The user's permissions aren't individually assigned, they derive only from their currently assigned role.