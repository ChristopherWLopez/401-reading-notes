# Class 16 - AWS

## What is an EC2 Instance?

Instances types comprise of different combinations of CPU, memory, storage, and networking capicity and gives you the flexibility to choose the correct mix of resources for your app.  Each instance type includes one or more instance sizes, this allows you to scale your resources to meet the requirements of your workload.

## Name 2 use cases for EC2

EC2 can be you server with the ability to scale especially as a new dev wher you dont know what your workload is going to be and how much it might fluctuate. And when you really might not have the funds to buy actual hardware.

Another instance is when you are creating an app that maybe requires people to be active at certain times, while the rest of the time its a mellow work load. AWS allows you to scale  as you need when you need

## Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com

I See that EC2 has alot more to offer. I think the scalability, The securrity, the ability to lesson your physical footprint there for you save on the hard ware (especially when you are not using it and the storage/ facility costs). You are also able to change you OS and other software as well as hardware when you create instances.... This means that you can adapt your server according to your app (patches) and the traffic needs. AWS really does have it all.

## Where can we find EC2 on the AWS Console?

Under the compute section.

## Explain the general difference between T2 Micro and XL

T2 is burstable which which allows you to earn burst credits. This means that you can burst above baseline CPU performance whenever you get a spike in traffic/ workload. (5%)

XL is a greater performing instance of the T2. The XL has greater storage and (2 : 8) this offers way better baseline performance (90%)

## Explain a “Compute Cycle” to a non-technical friend

This is the life cycle of our little helper robot. We create the littl guy and in that process we may have to way for him to be pieced together (this is our "pending" state). Once the our little robot friend is alive, We have him "running" when he is in this state he is up and running and ready to help us out or ready to hang out and do what little robots do best.... nap!... Okay maybe he is getting alittle sleepy so we are able to "terminate" him, That sounds worse than it is. We can shut him down and let him go to sleep for a while, or we could or we could terminate him.. Okay that does sound bad, but know that WHO that little robot is IS our program so we always have his being inside all we need to do is create a new instance of that little fella...GLOW UP time! I also want to say that we can "reboot" him which is like waking him up from a nap by letting him sleep off some grumpies.

## What is Elastic Beanstalk?

a service that deploys, manages and scales web apps for you.

## Describe the relationship between EC2 and Elastic Beanstalk

Elastic Beanstalk helps you manage your EC2 instances. This can keep track of our work load and can help us scale our instances as we need (be it up or down).

## Name some benefits of using Elastic Beanstalk

Elastic Beanstalk gives us the freedom to focus on the code and really focus on out code and app instead of the loadbalancing and automatic scaling

This helps us get to market faster by taking alot of the load off of our shoulders.

This is very easy because it comes at no extra charge, we can apply this amazing helper to our instances.

## overall notes

EBS - elastic block storage

security group - decide who can enter and who can exit (firewall)
