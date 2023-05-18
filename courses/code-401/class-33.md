# Reading 33 Notes

## What is Role Based Access Control (RBAC)?

### What is Role Based Access Control (RBAC)

RBAC is a methodology for restricting network access based on a person's role in an organizatoin

### Share some an example of RBAC including all possible CRUD operations and correlating roles

permissions methodology for my pokemon app written in week 2:

- GET     /pokemon      Lists all pokemon         Only pokemon masters and gym leaders have access
- POST    /pokemon      Creates new pokemon       Only pokemon masters and gym leaders have access
- GET     /pokemon/:id  Gets the :id pokemon      Pokemon masters, gym leaders, plus those trainers who have that pokemon have access
- PATCH   /pokemon/:id  Updates the :id pokemon   Pokemon masters, gym leaders, plus those trainers who have that pokemon have access
- DELETE  /pokemon/:id  Deletes the :id pokemon   Pokemon masters, gym leaders, plus those trainers who have that pokemon have access

adapted from here: https://www.toptal.com/firebase/role-based-firebase-authentication

### What are the Benefits of RBAC?

Reduces administrative work and IT support: reduce overhead, reduce password changes, switch roles quickly

Maximize operational efficiency: don't spend time performing lower level access control

Improve compliance: have a well defined security plan for sensitive data that withstands regulatory scrutiny

## Compare and Contrast the following two Libraries and the following questions. Yes, they are similarly named

### Describe some react-cookie features

- is a functional component
- access and modify Cookies using React Hooks
- has methods `get`, `getAll`, `set`, `remove`, that are self-explanatory

### Describe some react-cookies features

- is a class component
- has methods `load`, `loadAll()`, `select([regex])`, `save`, `remove`, `plugToRequest`. `setRawCookie`, that are not self-explanatory at all
- is version 1.04 of what is now react-cookie, with a couple changes. react-cookie is currently version 4.1.1 so react-cookies is ancient


### Which library would you prefer would you prefer? Why?

I would rather use react-cookie because it's a more modern interpretation, it's a functional component, and it doesn't require binding or class component state management, which I hate

react-cookies also hasn't been updated in 4 years and it's practically dead
