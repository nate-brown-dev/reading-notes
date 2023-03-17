# Code 301 Reading 15

## What is OAuth

### What is OAuth?

OAuth is a secure, third party, user agent, delegated authorization

### Give an example of what using OAuth would look like

- when you log onto a website and use another site's logon
- an example would be logging in to another page with your google account

### How does OAuth work? What are the steps that it takes to authenticate the user?

1. first website connects to second website on behalf of user, using oauth
2. second site generates one-time token and secret
3. first site gives token to user client
4. client presents request token to authorization provider
5. client might authenticate, and approve authorization to second website
6. user approves transation type at first website
7. user gets approved access token
8. user gives approved token to first website
9. first website gives access token to second
10. second lets first access it on behalf of user
11. user sees successful transaction occur

### What is OpenID?

OpenID is about authentication instead of authorizatoin

## Authorization and Authentication flows

### What is the difference between authorization and authentication?

authentication: prove who you are
authorization: prove you're allowed access to a resource

### What is Authorization Code Flow?

exchanges an authorization code for a token

### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

for single page apps, uses proof key for code exchange

### What is Implicit Flow with Form Post?

a version of OAuth for public clients, or applications which can't store client secrets

### What is Client Credentials Flow?

for back end apps, system authenticates and authorizes instead of user

### What is Device Authorization Flow?

for input constrained devices that access the internet/ IOT

### What is Resource Owner Password Flow?

highly trusted applications can use resource owner username and password, not recommended 

[Go back home](/reading-notes/)
