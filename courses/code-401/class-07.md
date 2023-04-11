# Code 401 Reading 7

## Intro to JWT

### What is a JSON Web Token (JWT)?

- JWT is a standard for secure information transmission
- information transmitted as JSON object
- digitally signed with secret or key

### When should we use JSON Web Tokens?

- authorization
  - after login, subsequent requests use token instead of login string
- information exchange
  - signed including header/payload
  - verifies header/payload have not changed since signing

### Claims are expected in which structural component of a JWT?

- claims go in the payload

## Are JWTs Secure?

### If I get a JWT and I can decode the payload, how can we call that secure?

- that's the point of sending a jwt with payload, so you can decode it
- the payload is sent as base-64, not encrypted
- the jwt just tells the receiver that the payload has not changed since it was signed
- if the payload and token don't match -> don't accept payload as valid

### If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature

- the sender and receiver have to know the secret
- the secret is appended in the signature

### Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter

- user authenticates in order to generate token
- to generate token, the header and payload are encoded base-64 and combined with the secret
- then the whole thing is encoded SHA 256 (one way hashing algorithm)
- token is sent back to user
- when user sends the token as authentication, the header and payload (cleartext) are combined wih the secret again by the receiver, and re-hashed
- if the hashes match, the token is valid because the header and payload haven't changed
- if the header or payload HAVE CHANGED, and combined with the secret, that new hash won't match the signature -> unauthorized

## Video: JWTs Explained

### Why use JWT?

- jwt is a way to prove that a message has not changed since it was signed
- when the signature is applied, the header/payload are frozen
- if the header/payload change, the signature is invalidated

### JWT is Compact and self-contained. Describe how this is useful to a non-technical friend

- the token is very small, so it takes little overhead (it's fast)
- it's self contained - the token itself contains the information about the user
- requests can be made using only the token, instead of token + user (simpler)

### What are the three components (the structure) of a JWT signature?

- base 64 encoded header
- base 64 encoded payload
- secret

then all 3 things are combined and hashed
