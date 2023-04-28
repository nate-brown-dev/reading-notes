# Code 401 Reading 19

## AWS SQS vs SNS

### What is the difference betweeen SQS and SNS?

SNS is a PUSH system - messages are sent to endpoints immediately

SQS is a PULL system = messages go in a queue, users have to ask for them

SQS can be used as an endpoint for SNS = messages to the the queue immediately and users ask for them later

### What are some use cases for both SNS and SQS?

SNS: multiple subscribers, batches of messages, process same message in multiple ways/endpoints

SQS: asynchronous processing, only one subscriber

## AWS SNS and SQS

### Describe how to use SQS and SNS in a “fanout” pattern

A single SNS topic takes multiple endpoints, some of which are SQS queues. These queues have differnent target audiences/pollers but take the same informatino from the SNS message

### Explain how “push notifications” work, using SNS

SNS interacts with push notification services on the receiving mobile device (ex Apple Push Notification Service on iOS)

The push notification services are connected/registerd to each app on the device that takes push notifications. SNS uses the device token to create a mobile endpoint

referenced here [https://docs.aws.amazon.com/sns/latest/dg/sns-mobile-application-as-subscriber.html](https://docs.aws.amazon.com/sns/latest/dg/sns-mobile-application-as-subscriber.html)

## SQS and SNS Basics

### How might a large scale, distributed application make use of a Queue system like SQS?

an example was in the previous video - for Amazon retail, a single completed notification (SNS) has multiple SQS endpoints, examples of this would be "leave a product review" queue, "order again" queue, queues for amazon employee QA / analytics. Combine this with many notification generators (customers) and you have lots of message traffic going to many queue endpoints
