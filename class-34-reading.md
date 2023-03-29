# Class 34 reading

## Explain the different between a query string parameter and a path parameter

The path parameter defines the resourse location while the query parameter defines `sort` and `pagination` (division of pages). The users query  gets placed (as a variable in the query) while the path parameter needs an actual page value to go to that page.

## What would our API URL with a path id parameter be given the following information

## Domain: <http://our-site.com>

## v3

## model name: stuff

## id: things

## We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend

Our Api interface is the meeting point between what the user is requesting and the actual database itself. It acts like a bouncer to an open bar. You can get what you want as along as you have what the bouncer requires.

## Describe how you would use middleware to implement basic and bearer auth

we would use  auth routes that would handle the log-in and authentication system.

Our middleware would handle the 404 and 500 conditions
and the middle ware would handle each type of authentication. Basic, OAuth, and Bearer

We run our middleware after Bearer Middleware on routes to be protected.

## Describe the handshake necessary to implement OAuth

The client will initiate a handshake in the browser (using a 3rd party authentication service).After the user is granted access we will invoke a `GET`  on our `/oauth` route. The OAUTH middleware should then complete the handshake process which would create/update a local user account in our database and then return an object containing our bearer token/ re-authentication and the `user object`.

## Describe how Role Based Access Control works to a non-technical friend

These are user roles and the abilities a user would have based on their role. These are predefined and assigned based on the role itself. These makes sure that every has access to only what they need to do their job.
