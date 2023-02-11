# Class-18

## What is Amazon API Gateway?

Amazon Api gateway is a service that lets us developers define our own endpoints for either REST API or Websocket API's and connect those end points to our corresponding business logic.

These sit between our API servers and our API users, we are able to use fully managed authentication, and authorization as well as metrics for our API requests.

## Why is Amazon API Gateway an important part of the Serverless ecosystem?

This tie together the serverless functions and the API definitions. We are able to trigger the execution of a serverless function in direct response to an HTTP request. This allows us to build a real time fully functioning app without maintaining a server ourselve.

scalability, low maintainence, and low cost.

## How does API Gateway integrate with other AWS services?

AWS lambda: Run a Lambda function to generate HTTP API responses.
AWS SNS: get notifications when the HTTP API endpiont is accessed.
Amazon Cognito: authentication/ authorization for HTTP API's.

 " Invoking an AWS Lambda function.
Invoking another HTTP endpoint, with or without VPC Link.
Making an HTTP call against the API of any AWS service that provides an HTTP API.
Returning a mock response generated within API Gateway without calling out to other services." [taken from serverless.com](https://www.serverless.com/guides/amazon-api-gateway).

## What are the some benefits of using Amazon API Gateway?

API gateway handles tasks like : accepting and processing alot of concurrent API calls, traffic management, CORS support, and authorization and access control, throttling, and monitoring, verion management.

## What two API types might you choose from?

RESTful APIs and WEBSOCKET APIs.

## What is DynamoDB?

DynamoDB is a  NoSQL database that is offered by AWS. It offers reliable, scalible performance, managed experience in a small simple API allowing for simple key-value access (and more advances query patterns).

## Under what circumstances would you recommend DynamoDB over MongoDB?

You would use DynamoDB when your DATA starts to scale, because JOINs and SQL operations can slow queries. When you use DynamoDB, your queries have predictable latency.

If you are using Serverless applications like AWS Lambda (auto scaling, stateless... amazing web service).

## Explain to a non-technical friend how DynamoDB works

DynamoDB is a very flexible self maintaining Database that can hold data with no specific structure which would give us the ability to easily define the structure of the data.

This service has alot of built in features like built in security, automatically backs up your data and can store that info (in house). This is like having a library that is able to check and make sure that anyone who enters and wants data is who they say they are and they have the correct creditentials. This also has the ability to add more rooms as you need. When you use this service you are connected to a new work of construction workes (to add to your library) and other libraries to help you store and or manage your books (data).

This is like being involved with a big organization that really does alot of the heavy lifting for you.

## What is Dynamoose?

This is a modeling tool that is made for AWS's DynamoDB... This IS INSPIRED by mongoose.

## What are some key features of Dynamoose?

Type Safety
Highlevel API
Easy to use syntax
DynamoDB single table design support.
can transform data before saving or retrieving.
"strict" data modeling.
support for DynamoDB transactions.
callback/ promise support
multi-region support.

## Things I want to know more about

what is throttling?

I really want to understand the triggering of the Lambda functions. I know we will touch on this with the API request, but I want to better understand this.
