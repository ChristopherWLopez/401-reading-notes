# Class 7 reading

## What is a JSON Web Token (JWT)?

A JWT is a digitally assigned compact way to securely transmit info between parties as a JSON object. These can be assigned by using a HMAC algorithm.

There is a way to make these ecrypted which would "provide secercy between parties and they could be signed to varify the "integrity" by being signed by "public/private pairs". This also certifies that the holder is who the one who signed it.

## When should we use JSON Web Tokens?

**Authorization** : This is great for when the user is logged in and each request after the fact will allow the user "access" to the routes and other features that token is permitted to use.

**Information Exchange** : This speaks for when the token has been signed by using public and private key pairs. This means you can be sure that the user is who they say they are.

## Claims are expected in which structural component of a JWT?

The "pay load" would be the part to hold the claims. The claims are "statements" about the entity that is using it, and other data.

 **Registered claims** This is a set of claims that are predefined but not mandatory such as: *iss*(issuer),*exp*(expiration time), *sub*(subject),*aud*(audience)... there are others.

## Token structure

The web token structure has a Header, Payload, and a Signature so it looks like this. `xxxxx.yyyyy.zzzzz`

The Header: is made up of two parts... the token type and the signing algo (HMAC, SHA256, RSA).

Payload: This contains the claims. Claims are statements about the entity and other info. There are different types of claims.

## If I get a JWT and I can decode the payload, how can we call that secure?

tokens are either signed or encrypted or both. If the token is signed for (and not ecrytped) than everyone can see its contents, however the signature (key) still must be what it is and it must match.

## If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature

They must know the "secret" also known as the key. this a part of a "formula" that takes place and must be correct in order for the hash function `hash(payload + secret)` this means that if you dont know the secret you will not get the correct signature.

## Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter

The two pieces of information "content" (this actual content) plus the "secret" are two pieces being placed inside a function that will place these two things together and then do specific things to them, then to output the information as along series of numbers/letters. The content itself isnt a secret but of course the secret is, there for getting those series of numbers and altered content to match seems incredibly difficult to do.

## Why use JWT?

This used to securely transfer between any two bodies. The info is digitally signed and varified.

## JWT is Compact and self-contained. Describe how this is useful to a non-technical friend

This is like throwing a car. JWT is a small sports car that has more access to more streets and roads than a tank would. A tank could not just drive down a regular street or freeway. There are more limitations on the tanks and how mobile it is.

## What are the three components (the structure) of a JWT signature?

The header:

 a JSON object. this consists of the algorithmn and the type of token

Payload:

 This contains the user details or any meta data. This is base64 encoded

The signature:

 This helps to ensure the info isnt changed between the two bodies. The signature itself uses algorithmns to encode the header and the payload, these two components added with the secret creates a JWT.

### Reflection

I am interestedin learned more about web security. I think this is a very interesting topic that I would like to learn more about. 

## notes

JWT doesnt care about encryption its main focus is validation. With this in mind and having the correct hashfunction on had this means that it can check if anything has been tampered with, therefore the validation will not work.

 we start with a post request from the client to the server with the credentials
 the server generates the JWT w/ the secret
 this is passed back to the browser. If successful JWT
 This is sent back(server) on the auth. header, This gets checked, if JWT signature matches then you are granted access to resources.
 the resources are sent back.

 It looks like all the info is built ontop of eachother. The signature is made up of the contents being a certain way,so the contents are important.


### Things I want to know more about

A Deeper dive into claims.
