# Code 401 Reading 18

## AWS API Gateway Overview

### What is Amazon API Gateway?

- service that defines HTTP endpoints and connects them with backend logic
- also connects authentication, access control, monitoring, tracing

### Why is Amazon API Gateway an important part of the Serverless ecosystem?

- it connects the serverless functions to API definitions
- it connects all the pieces of the serverless ecosystem to the users

### How does API Gateway integrate with other AWS services?

- Some AWS services are directly integrated with API gateway user interface, or via Gateway API
- for non-directly integrated services, can connect through HTTP endpoints

## AWS API Gateway

### What are the some benefits of using Amazon API Gateway?

- efficient development
- easy monitoring
- flexible security controls
- restful api options

### What two API types might you choose from?

- HTTP APIs
- REST APIs

## AWS DynamoDB Guide

### What is DynamoDB?

AWS hosted NoSQL database

### Under what circumstances would you recommend DynamoDB over MongoDB?

- Dynamo DB will scale more effectively with less performance cost
- Dynamo DB can scale automatically instead of intentionally adding/migrating instances, and it can scale down too, instead of being stuck with capacity you aren't using
- Dynamo DB works better with serverless computing / Lambda

## AWS DynamoDB

### Explain to a non-technical friend how DynamoDB works

- Dynamo DB is a document model database, which means it's a table with a bunch of rows that have no relationship to each other
- each row can have any number of columns
- each row can be different than any other row
- imagine making an excel sheet, and putting whatever you want in each row
- you can't use the rows to execute functions on each other but you can scribble away however you like

## Dynamoose

### What is Dynamoose?

Dynamoose is a modeling tool for Dynamo DB, like Mongoose for MongoDB

### What are some key features of Dynamoose?

- Type safety
- Transform data before saving/retrieving
- Strict data modeling, validation, required attributes
- Transactions
- Conditional Filtering
- Callback/promise support

[Go back home](/../reading-notes/)
