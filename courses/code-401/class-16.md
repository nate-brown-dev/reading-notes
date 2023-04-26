# Code 401 Reading 16

## AWS EC2

### What is an EC2 Instance?

- an "instance" is the virtual server that AWS provides for your program to run on
- AWS provides the hardware and bandwidth that runs your product
- instances have varying combinations of CPU, memory, storage, and networking capacity
- instances can be scaled to target workload

### Name 2 use cases for EC2

- compute optimized instance use cases
  - high performance web servers
  - high performance computing
  - scientific modeling
  - gaming servers
  - machine learning interface

- accelerated computing
  - floating point calculations
  - graphics processing
  - data pattern matching

### Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com

resource allocation is AWS is dynamic and can adapt to demand spikes, but you don't have to pay for large bandwidth all the time

## EC2 For Humans

### Where can we find EC2 on the AWS Console?

In the AWS console, all services > compute

### Explain the general difference between T2 Micro and XL

They are just different tiers of power/memory/storage for the EC2 instance

### Explain a “Compute Cycle” to a non-technical friend

- "compute cycle" in a cloud context is a metric that describes how much processing power your app is using
- your app isn't using the entire capacity of the data center server processor at any given time, or ever, it's using some amount of "compute cycle"
- you pay for the amount of compute cycle you are using

### What is Elastic Beanstalk?

an AWS service that deploys and scales web servers for you

### Describe the relationship between EC2 and Elastic Beanstalk

- Elastic Beanstalk is an environment in which you can have multiple EC2 instances
- EB automates setting up AWS services

### Name some benefits of using Elastic Beanstalk

- EB automates setting up AWS services
- EB keeps you from spending lots of time doing sys admin tasks like load balancing
- It lets you devote your time to your app instead

[Go back home](/../reading-notes/)
