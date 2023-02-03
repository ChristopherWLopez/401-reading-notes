# class 17 reading

## What is Amazon S3?

An object storage serive that offers scalability, security, and data availibality. This is key value store which is a big feature in a NoSQL database.

## Name some use cases for Amazon S3

Data Analytics

machine learning

A overall data base where you can scale your storage accordingly.

## Name some benefits of using Amazon S3

S3 can scale according to your needs, it makes it easy tp retrieve data ("Meet Recovery Time Objectives (RTO), Recovery Point Objectives (RPO), and compliance requirements with S3’s robust replication features.").

Remove operational complexitys which allows you the ability to just focus on the task at hand (the code) instead of worrying about the infrastructure.

It is easy to configure. so you can personalize your needs for whatever task you are working on.

## What is AWS Lambda?

Lambda is a computing service that is supplied by aws. They state they are a serverless service, however you are able to host servers, and make API calls. The dea pd it being a "serverless service" means that all  that stuff "the hosting/ serving" is already managed by the company So as coders we focus on the code and creating the functions that we need to and leave the infrastructure maintanence to those fine folks at AWS.

## Name some use cases for AWS Lambdas

Aws lambda is a service that allos us to store our functions inside of containers and these containers are run and then amount of storage and CPU that is required to make these run are noted and we are charged for it as we need.

scalable API's where one execution of a lAMBDA function can serve a single HTTP request. Also different calls can be routed to different functions via the AWS gateway. The individual functions also get scaled based off of their use.

## Describe “serverless” to a non-technical friend

ServerLess refers to use not having to maintain our own servers. We are able to write the code for our servers and make sure that ther doing what we want... however we do not need to maintain them!  they are maintained by those awesome people who work for AWS so for us as developers we just focus on the code at hand. Usually when we create a server there is alot to worry about. Its kind of like being a cook.When we are runng our own sever we need to prepare the food, chop every thing and get all the measurements correctly... when we use Lambda we are just the cook, we have people helping us prep and maintain things so if we need to make more food we dont need to chop dozens of onions... all we do it keep cooking the main meals and take what we are given.

## What is a CDN?

A CDN (content delivery network), is a group of geographically distrubeted servers that all work together to provide fast delivery of internet content. This offers a fast transfer of data that is needed for loading internet content like HTML, Javascript, images, etc...

## How does a CDN work with relation to the website visitor?

When a client visits a website they would usually make requests to a specific server. This can be a problem if the user and the server are on opposite sides of the country or even the world, this could impact speed. However with CDNs there is able to be a group of servers that have the same data as the original server however now the client can request the info and get the response from a server that is much closer to them, this server holds the same data it just makes it much faster and easier since we do not need to worry about communicating from client and server that has a huge inbetween them.

## What are the benefits of employing a CDN?

using a CDN offers quicker loadtimes as well as helping against cyber attacks DDos attacks, it protects against these threats because CDNs are spread out over many servers we do not have all traffic being sent to one central server... so we do not have too many requests going through.

I am pretty excited to dig into auto scaling functions (by using Lamba). This seems like a pretty cool concept that I would like to see in action.

### Things I want to know more about

I really want to dig into this whole "serverless functions"