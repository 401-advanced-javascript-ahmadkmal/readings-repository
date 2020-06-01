# read 6

## HTTP & REST

### HTTP

The Hypertext Transfer Protocol (HTTP) is designed to enable communications between clients and servers.

HTTP works as a request-response protocol between a client and server.

Example: A client (browser) sends an HTTP request to the server; then the server returns a response to the client. The response contains status information about the request and may also contain the requested content.

#### HTTP Methods

GET
POST
PUT
HEAD
DELETE
PATCH
OPTIONS
The two most common HTTP methods are: GET and POST.

#### HTTP status 

When a browser requests a service from a web server, an error might occur, and the server might return an error code like "404 Not Found".

It is common to name these errors HTML error messages.

But these messages are something called HTTP status messages. In fact, the server always returns a message for every request. The most common message is 200 OK.

Below is a list of HTTP status messages that might be returned:

1xx: Information
2xx: Successful
3xx: Redirection
4xx: Client Error
5xx: Server Error

### REST

Representational State Transfer
is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other. REST-compliant systems, often called RESTful systems, are characterized by how they are stateless and separate the concerns of client and server. We will go into what these terms mean and why they are beneficial characteristics for services on the Web.