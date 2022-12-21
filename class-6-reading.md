# Class 5 reading

## Explain to a non-technical friend how you would safely hash and store a password

It is best to create a function that will "hash" (jumble up the password) in order to make it unknown to prying eyes. There is a common tactic people use to try and crack passwords and this function that we create would make it incredibly hard to crack.

## What is Bcrypt?

Bcrypt is a function that we would use to encrypt and salt our password. It is also "adaptive" which means that it can slow down and while computers speed up this function can stay slow or go even slower which can help against "BRUTE FORCE" attacks.

## Why might you use something like Bcrypt?

Bcrypt are great against bruteforce attacks and this allows us to adjust the speed of our hash which would help keep our passwords safe.

## What is Basic Authentication?

BSA is a method for a brower or HTTP "...user agent to provide a user name and password when making a request.

## What properties are necessary in the header of a Basic Auth request?

Cache Credentials

## How are username:password in Basic Auth encoded?

They are encoded with Base64 ["This is a group binary-to-text encoding schemes that represent binary data"](https://en.wikipedia.org/wiki/Base64) This goes along with HTTPS.
[info-from-wiki](wikipedia.org)

### notes Basic AUTH

- BA does not provide confidentiality protection for transmitted credentials they are encoded with `Base64` IN TRANSIT. these are not encrypted or hashed. This pairs with HTTPS to provide confedentiality.

- Gets sent through header.

- each HTTP request needs to be cached credentials for a reasonable amount of time, So user doesnt get bother to re sign-in.

- cache credentials are often cleared when browser history is cleared.

-

## Define the authentication process to a non-technical recruiter

This is the process of the user proving that they are who they say they are, This is commonly done by asking for user name and password and another piece of info that only the user would know.

## How should your error messaging respond (both HTTP and HTML)? Why?

Error messages should be generic and logged to the server to be investigated. There are some instances where an error message can even give more info and make it possible to be logged into against the real users will.

## Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle

### OWASP notes

**Authentication**  is a user proving that they are who they say they are, This is often done by asking for "username" and "password" and sometimes another peice if into that only the user would know.

**Session Management** This is the process of the serverm MAINTAINING the state  of an "entity" that is interacting with it. This means that the server needs to remember how to react based on what user is using it. This gets passed back and forth between  client and server.

- make sure your usernames and ID are case sensitive.
- they should be unique.
- in high security they should be issued and not user defined.

- dont allot login to back-end/ middleware.

### OWASP [cheat-sheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)

I am pretty interested in the Role Based access control aspect of this module. I cant say I know exactly what that entails but it does sound pretty awesome.

I want to get a better grasp on cipher algo's i did attend a meet up where we discussed a certain cipher and I thought it was pretty neat.

### Things I want to know more about

- I think alot of my questions might be answered if I am able to parse the bcrypt documents. I can kind of understand what we are trying to do but this "art" is so big that I dont know if i would be able to even know where to begin.