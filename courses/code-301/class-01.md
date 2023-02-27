# Code 301 Reading 1

## Component-Based Architecture

### What is a “component”?

definition from https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm

- a modular, portable, replaceable, reusable set of functionality
- a software object that interacts with other components
- a unit of composition with specific interface and dependencies only

### What are the characteristics of a component?

list from above site

- reusability
  - can be used in different situations for different tasks
- replaceability
  - can be substituted with other components
- not context specific
  - operate in diff environments
- extensible
  - new behaviors can be added
- encapsulated
  - don't expose internal variables or state to user
- independent
  - minimal external dependencies

### What are the advantages of using component-based architecture?

list from above site

- ease of deployment
- reduced cost
- ease of development
- reusable
- modified technical complexity
- reliability
- ease of maintenance/evolution
- independent

## What is Props and How to Use it in React

### What is “props” short for?

- properties

### How are props used in React?

- props are used to pass data from parent to child components
- props data is read only

### What is the flow of props?

- props are passed one-way from parent to child components
- props work like function arguments
- props are read-only data

[Go back home](/reading-notes/)
