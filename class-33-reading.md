# Class 33 reading

## What is Role Based Access Control (RBAC)?

It is a way to restrict network access based on a persons role within an organization.

## Share some an example of RBAC including all possible CRUD operations and correlating roles

An Admin would be able to create, update, delete and read.
An Editor would be able to update and read
A writer would be able to create and read
A customer of the paper would only be able to read the paper.

## What are the Benefits of RBAC?

This can reduce administrative work as well as IT support. You are able to assign an employees resposibility as they are hire and an can transer that roll if they are terminated. By doing it this way you are assuring that employees are focusing only on their work and nothing else that could be considered a "conflict of interest" (giving everyone access to payroll).

There is also the fact that helps meet federal, state, and local regulations. This ensures that companies are meeting requirements for privacy and confidentiality.

## Describe some react-cookie features

in order to set the cookies (on the server) the props must be set using `req.universalCooies`
You are able to both access and modify the stored cookies via react hooks.
With dependencies you are able to specify a list of cookie names your component depeneds on OUR ones that should trigger a re-render.
When setting your cookie you can also set `options` (besides the name and value). You can set the path, what date you want your cookies to expire, max age(?) amongst many other features, you can state if it is secure (only through `https`).

you can remove the cookie.

## Describe some react-cookies features

You are able to load the userId on mount (when we get our initial rendering)
You are able to tokenize the users cookies.
The ability to use regex to mathch all the cookies with the same name.
You can use `.plugToRequest(req,rea):unplug()` to do server-rendering..
compatible with `express.js`


## Which library would you prefer would you prefer? Why?
