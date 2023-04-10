# Code 401 Reading 6

## Securing Passwords

### Explain to a non-technical friend how you would safely hash and store a password

- password hashing is like putting the password through a one-way valve
- you make the password letters out of cake frosting
- then you put all the frosting letters in a tube with a decorative tip
- then you squeeze it out into the storage area
- what comes out doesn't look anything like the original letters

### What is Bcrypt?

- Bcrypt is an adaptive hash function
- Bcrypt based on Blowfish symmetric block cipher
- Bcrypt introduces work factor for determination of how expensive hash function will be

### Why might you use something like Bcrypt?

- If your site has to store user passwords
- If the site stores other sensitive user data
- If your site is likely to face brute-force attacks

## Basic Auth

### What is Basic Authentication?

- Basic authentication is a method of sending user credentiails (username/password) as HTTP header
- the username and password are sent as unencrpted strings
- basic auth normally used with HTTPS

### What properties are necessary in the header of a Basic Auth request?

- the header line is titled `Authorization: Basic`
- the username and password are separated with colon `username:password`
- username and password cannot include `:`

### How are username:password in Basic Auth encoded?

- the string of combined username and password is encoded in octet
- character set is unspecified, must be compatible with US ASCII, can be UTF-8
- octet string encoded as Base64 (with padding if required, `=` used for padding)
- 'Authorization: Basic' added to front of string

## OWASP auth cheatsheet

### Define the authentication process to a non-technical recruiter

- user goes to web site
- web site prompts user for credentials, or redirects to authentication provider
- user provides credentials
- web site / authentication provider checks that credentials are valid (authentication)
- if authenticated, return to web site

### How should your error messaging respond (both HTTP and HTML)? Why?

- error messaging should return errors in a way that takes the same time for wrong usernames and passwords
- this prevents intruder from distinguishing incorrect username vs password
- error messaging should not return error codes in a way that allows it to be used for the same things
