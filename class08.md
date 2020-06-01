# class08

## Express Routing & Connected API

### Express Routing

Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing, see Basic routing.

You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function (See Using middleware for details).

These routing methods specify a callback function (sometimes called “handler functions”) called when the application receives a request to the specified route (endpoint) and HTTP method. In other words, the application “listens” for requests that match the specified route(s) and method(s), and when it detects a match, it calls the specified callback function.

In fact, the routing methods can have more than one callback function as arguments. With multiple callback functions, it is important to provide next as an argument to the callback function and then call next() within the body of the function to hand off control to the next callback.

#### Route methods

A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.
Express supports methods that correspond to all HTTP request methods: get, post, and so on

### index.js

is where the apllecation start and it control of reunningthe server and it prameter

### server.js

it handel ever thing in the server include the route metode and the errore hundler and it have the mudels and middleware to run

### Data Model

The Data Model (DM) deals with entities at the database level. Like how the classes in the object model will get stored and in which tables. So, DM deals with table schema and the relationships between different tables

