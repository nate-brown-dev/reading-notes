# Code 401 Reading 2

## An introduction to NodeJS and Express

### Explain middleware, answer as though I were a non-technical recruiter

- middleware is software that fills in the gaps between applications, users and data
- in cloud computing, middleware glues everything together like connective tissue
- in express, middleware adds functionality that doesn't exist in the base package, to address different kinds of web development problems

### Express the most popular ________ ?

Express is the most popular Node web framework

### Express is “unopinionated.” What does that mean?

- It means that Express doesn't specify the "right way" to do something
- Developers using express can choose whatever components they want to solve their problem and Express is ok with it

### What is a module and why is modularity useful to us as developers?

- A module is a component that performs a specific purpose
- Modular components can be re-used
- Modularity makes code maintenance easier

## What is NPM?

### What version of npm are you running on your machine?

npm 9.5.0

### What command would you type to install a library/package called ‘jshint’ into your node project?

npm install jshint

## What is TDD?

### Explain why tests are important. Please explain as though I were your non technical elder

tests allow the developer to assess functionality when a program is not actually serving users

### What are three expected benefits of testing

- reduce defect rates: spending time to use tests during early development takes more work but results in better product
- reduce effort in late stages: along with above, if tests result in making a good product from the beginning, later work is easier
- test driven development can lead to better code quality

### Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests

- Individual
  - not running tests regularly
  - trying to write too many tests at once

- Team
  - Inconsistent adoption, not everybody on board with tests
  - tests not maintained, or abandoned

## CI/CD

This video is unavailable because the user closed their Youtube account

### What are three benefits of Continuous Integration?

- iterate faster: easier to manage compared to large feature releases spaced out over months/years
- find problems easier: easier to find bugs in small batches of code, and fix them
- make users happy: better code quality from CI makes better products

### What is the difference between Continuos Delivery and Continuous Deployment?

- continuous integration is something that happens at the developer level
  - each developer on a project merges multiple times per day
  - thus each developer always has an almost-current version of the product
- continuous delivery is something that happens in production
  - releases are automatically built, tested, and deployed

### Explain how GitHub fits into this process assuming the listener comes from a non-technical background

- Github is a central hub where developers on a project collaboratively work on a single project
- It allows the developers to work together, review each others work, decide what to keep or discard
- It saves everything so that developers always have access to the project
