# Class 3 reading

## Classes are a template for creating ____

**Objects**

## Can a class declaration be hoisted?

No, ["...They must be defined before they can be constructed..."](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes) This happens because the **values** are not "initialized"

## How would you describe a constructor and contextual “this” to a non-technical friend?

A constructor is like factory that creates people/"objects" each item is made individually however each person does have its own "properties" which is like (for me) my name property = "chris" or my eyes property os equal to "brown". So each person / object made has its owbn special qualities. We also use "contextual THIS" which is how we refer to the specific item at hand. say you pick up a flower. You can pick generalize and say "sunflowers are yellow" but the "contextul this" refers to the flower you have in your hand at that moment.. it refers to THAT FLOWER. so you could say `this.color = yellowish orange" you can be more specific and it just points to that item.

## Within Express, what does routing refer to?

This refers to how an apps "end point" responds to a clients request.

## What is the difference between a route path and a route method?

A route method is derived from one of the HTTP methods. This gets attached to the instance of express that we initialize at the top of the script. e.g...`app.get()`

while.. The rout path is the actual path that is being defined in the rout method. This is our "home route" `/` or even `/users` this would be followed by our callback function that was stated above (in route method section).

## When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?

This is handy when you use more than one callback function within your method. You would use the `nexy()` method to hand the rout to the next function to finish the job. This also assures thaat we by pass the remaining the route callbacks. This can be used to "impose preconditions on a route, then pass control to subsequent routes if there is no reason to preceed with the current route" [taken from expressjs.com](https://expressjs.com/en/guide/routing.html)

## What is an Express Router?

This is a "mini-Express application.... .... This provides us with routing API's like: .use,, .get, .param, and route." [taken from **digitalocean**](https://www.digitalocean.com/community/tutorials/learn-to-use-the-new-router-in-expressjs-4).

## By what mean do we initialize express.Router() in an express server?

This means that we assign an instance of `express.router()` to a variable so that we can use that variable and assign route methods to that variable... in my experience we have used `app` as the initiallzed variable. The `express.router()` is a "mini express app in its simplest form.

## What do we use route middleware for?

This is way to do something like "authenticate" or even display (or just do something) "...before the request is processed..." This could "analytics" or data logging. In this article `app.use()` was the method was used with three parameters `(req, res, next)` 

`    // route middleware that will happen on every request
    router.use(function(req, res, next) {

        // log each request to the console
        console.log(req.method, req.url);

        // continue doing what we were doing and go to the route
        next();
    });

    // home page route (http://localhost:8080)
    router.get('/', function(req, res) {
        res.send('im the home page!');
    }); `


### General Notes

You can have class expressions and class declarations and class expressions.

Class declaraction can be declared using class keyword.

"You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function"[taken from here express.js](https://expressjs.com/en/guide/routing.html)

You can use multiple callback functions however if you choose to do so then you would need to call the `next()` method to signify the next callback.

We could us `app.use()` to define out middleware.

### Things i want to know more about

I want to know more about the `.all()` method in express.

I want to look up the proper use of the `next()` method and see its functional uses.

when using middleware and spitting out the users `req.method` and the `req.url` to the console why is it that we required to use `next()` ?

In the example on :

`...

    // we'll create our routes here

    // get an instance of router
    var router = express.Router();

    // route middleware that will happen on every request
    router.use(function(req, res, next) {

        // log each request to the console
        console.log(req.method, req.url);

        // continue doing what we were doing and go to the route
        next();
    });

    // home page route (http://localhost:8080)
    router.get('/', function(req, res) {
        res.send('im the home page!');
    });

    // about page route (http://localhost:8080/about)
    router.get('/about', function(req, res) {
        res.send('im the about page!');
    });

    // apply the routes to our application
    app.use('/', router); `

why is the middleware happen on every request?
